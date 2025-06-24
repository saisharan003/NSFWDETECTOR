# 📄 NSFW Image Content Moderator — AI + Human Review (Google Colab)

This mini-project demonstrates an AI-powered content moderation workflow for detecting NSFW (Not Safe For Work) images using a pre-trained deep learning model. It integrates automated detection with manual moderator decisions to replicate real-world trust & safety pipelines.

🔗 Try the project now on Colab:  
https://colab.research.google.com/gist/saisharan003/91e085e994e26bbb47771143f034fc7f/nsfwdetector.ipynb

---

## 📌 Features

✅ Upload any image via Colab interface  
✅ Use OpenNSFW2 (pre-trained model) to detect NSFW probability  
✅ Classify images:
- Score ≥ 0.7 → Flagged for review  
- Score < 0.7 → Auto-approved  
✅ Moderator can override AI decision (Approve/Reject)  
✅ Simple Python logic with clean interface for demo/testing

---

## 🧠 Tech Used

| Tool | Purpose |
|------|---------|
| opennsfw2 | NSFW detection using deep CNNs |
| Pillow (PIL) | Image reading and conversion |
| Google Colab | Free GPU-powered IDE and easy shareability |
| Python 3 | Core scripting and moderation logic |

---

## 🎯 Why This Project?

This project showcases core responsibilities of a content moderator:

- Understanding and interpreting AI content scores  
- Making judgment calls on borderline content  
- Combining AI automation with human oversight  
- Flagging and documenting moderation decisions

It simulates the real-world balance between automation and manual safety review seen on platforms like Meta, YouTube, and Reddit.

---

## ⚙️ How It Works

1. Upload an image using the Colab upload widget  
2. Model analyzes and returns a NSFW probability (0 to 1)  
3. Based on threshold:
   - If ≥ 0.7 → flagged for review  
   - If < 0.7 → auto-approved  
4. User (you, the moderator) manually enters final decision

---

## 📂 Example Output

```
📊 NSFW Score: 0.82
🚩 Flagged for review (score ≥ 0.7)
Manual decision? Type 'approve' or 'reject': reject
✋ You rejected this image.
```

---

## 📈 Future Improvements

- Add CSV logging of decisions  
- Visual UI using Streamlit  
- Include additional models (e.g., Blur nudity detection, violence scoring)  
- Multiple image upload support

---

## 📣 Credits

- opennsfw2: https://github.com/ebekkouche/opennsfw2  
- PIL: Python Imaging Library  
- Google Colab: Free cloud compute environment
