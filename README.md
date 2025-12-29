🧩 PART 1 — Title + One-line description

Paste this at the top 👇

# LeRobot PushT – ACT Policy Evaluation

This repository contains training checkpoints, evaluation videos, and notes from running the ACT policy on the PushT environment using Hugging Face LeRobot.


🔹 This tells what the repo is
🔹 Clear, simple, no buzzwords

🧩 PART 2 — What you actually did

Add this below 👇

## What This Project Demonstrates

- Offline training of an ACT (Action Chunking Transformer) policy
- Evaluation on the PushT-v0 manipulation environment
- CPU-based execution using WSL (Ubuntu)
- Video-based qualitative analysis of agent behavior


🔹 Shows skills, not just results
🔹 Anyone reading knows this was hands-on

🧩 PART 3 — Repo structure (very important)

Add this 👇

## Repository Structure


lerobot-pusht/
├── checkpoints/
│   └── 000100/
│       └── pretrained_model/
│
├── results/
│   └── eval_videos/
│       ├── eval_episode_0.mp4
│       ├── eval_episode_1.mp4
│       └── eval_episode_2.mp4
│
├── notes/
│
├── .gitignore
└── README.md


🔹 Reviewers LOVE this
🔹 Makes your repo readable in 5 seconds

🧩 PART 4 — Training details (simple, honest)

Add this 👇

## Training Details

- Environment: PushT-v0
- Policy: ACT
- Backbone: ResNet-18 (ImageNet pretrained)
- Training steps: 100 (demo run)
- Device: CPU
- Dataset: lerobot/pusht


⚠️ Saying “demo run” is GOOD — it shows honesty and awareness.

🧩 PART 5 — Evaluation results

Add this 👇

## Evaluation

- Episodes evaluated: 3
- Success rate: 0%
- Evaluation time: ~2.5 seconds per episode
- Outputs include rollout videos and reward metrics

Note: Low success is expected due to very limited training steps. The goal of this project is to demonstrate the full training → evaluation → visualization pipeline.


🔥 This line is important:

“demonstrate the full pipeline”

That’s exactly what you achieved.

🧩 PART 6 — How to reproduce (optional but powerful)

Add this 👇

## How to Reproduce

Training:

python src/lerobot/scripts/lerobot_train.py \
  --env.type pusht \
  --policy.type act \
  --dataset.repo_id lerobot/pusht \
  --policy.repo_id local/pusht-test \
  --steps 100


```markdown
Evaluation:

python src/lerobot/scripts/lerobot_eval.py \
  --env.type pusht \
  --policy.type act \
  --policy.pretrained_path checkpoints/000100/pretrained_model \
  --eval.n_episodes 3 \
  --eval.batch_size 3 \
  --env.render_mode rgb_array

```

🔹 Shows **reproducibility**  
🔹 Huge plus for interviews / reviewers

---

## 🧩 PART 7 — Closing (short & mature)

Add this 👇

```markdown
## Notes

This project focuses on understanding policy behavior through evaluation videos rather than achieving high task success. It serves as a foundation for further experimentation with longer training runs and GPU acceleration.
```

---

## ✅ Save & exit nano

Press:
```
CTRL + O → Enter
CTRL + X
```

---

## 🌟 What you now have

- A **real ML project README**
- Not flashy, but **serious**
- Perfect for GitHub, college, or future internships

---

### Next step options (pick one):

4️⃣ Create GitHub repo under **santhanuss** using `gh`  
5️⃣ Improve results (longer training / smaller model)  
6️⃣ Explain the videos *frame-by-frame* in simple language  

Just reply with the number 😼

give me a eady readme file

Got you 😼💙
Here is a READY-TO-USE README.md — clean, simple, and professional.
You can copy-paste this entire thing directly into your README.md.

# LeRobot PushT – ACT Policy Evaluation

This repository documents a complete training and evaluation pipeline using the ACT (Action Chunking Transformer) policy on the PushT environment with Hugging Face LeRobot.

The focus of this project is understanding policy behavior through evaluation videos rather than achieving high task success.

---

## What This Project Shows

- Offline training of an ACT policy on PushT-v0
- End-to-end workflow: training → checkpointing → evaluation
- CPU-based execution using WSL (Ubuntu)
- Qualitative analysis using rollout videos

---

## Repository Structure



lerobot-pusht/
├── checkpoints/
│ └── 000100/
│ └── pretrained_model/
│
├── results/
│ └── eval_videos/
│ ├── eval_episode_0.mp4
│ ├── eval_episode_1.mp4
│ └── eval_episode_2.mp4
│
├── notes/
├── .gitignore
└── README.md


---

## Training Configuration

- Environment: PushT-v0
- Policy: ACT (Action Chunking Transformer)
- Vision Backbone: ResNet-18 (ImageNet pretrained)
- Dataset: lerobot/pusht
- Training steps: 100 (demo run)
- Device: CPU

---

## Evaluation Results

- Episodes evaluated: 3
- Success rate: 0%
- Average episode time: ~2.5 seconds
- Outputs:
  - Rollout videos (`.mp4`)
  - Reward and timing metrics

Low success is expected due to the very limited number of training steps.  
The goal is to validate the full evaluation and visualization pipeline.

---

## How to Reproduce

### Training

```bash
python src/lerobot/scripts/lerobot_train.py \
  --env.type pusht \
  --policy.type act \
  --dataset.repo_id lerobot/pusht \
  --policy.repo_id local/pusht-test \
  --steps 100

Evaluation
python src/lerobot/scripts/lerobot_eval.py \
  --env.type pusht \
  --policy.type act \
  --policy.pretrained_path checkpoints/000100/pretrained_model \
  --eval.n_episodes 3 \
  --eval.batch_size 3 \
  --env.render_mode rgb_array

Notes

This repository is intended as a learning and experimentation project.
Future improvements include longer training runs, GPU acceleration, and policy tuning for higher success rates.


---
# LeRobot PushT – ACT Policy Evaluation

This repository contains training checkpoints, evaluation videos, and notes from running the ACT policy on the PushT environment using Hugging Face LeRobot.

## What This Project Demonstrates

- Offline training of an ACT (Action Chunking Transformer) policy
- Evaluation on the PushT-v0 manipulation environment
- CPU-based execution using WSL (Ubuntu)
- Video-based qualitative analysis of agent behavior
## Repository Structurelerobot-pusht/
├── checkpoints/
│   └── 000100/
│       └── pretrained_model/
│
├── results/
│   └── eval_videos/
│       ├── eval_episode_0.mp4
│       ├── eval_episode_1.mp4
│       └── eval_episode_2.mp4
│
├── notes/
│
├── .gitignore
└── README.md

## Training Details

- Environment: PushT-v0
- Policy: ACT
- Backbone: ResNet-18 (ImageNet pretrained)
- Training steps: 100 (demo run)
- Device: CPU
- Dataset: lerobot/pusht
## Evaluation

- Episodes evaluated: 3
- Success rate: 0%
- Evaluation time: ~2.5 seconds per episode
- Outputs include rollout videos and reward metrics

Note: Low success is expected due to very limited training steps. The goal of this project is to demonstrate the full training → evaluation → visualization pipeline.
## How to Reproduce

Training:
python src/lerobot/scripts/lerobot_train.py \
  --env.type pusht \
  --policy.type act \
  --dataset.repo_id lerobot/pusht \
  --policy.repo_id local/pusht-test \
  --steps 100

```markdown
Evaluation:
python src/lerobot/scripts/lerobot_eval.py \
  --env.type pusht \
  --policy.type act \
  --policy.pretrained_path checkpoints/000100/pretrained_model \
  --eval.n_episodes 3 \
  --eval.batch_size 3 \
  --env.render_mode rgb_array
```

🔹 Shows **reproducibility**  
🔹 Huge plus for interviews / reviewers

---

## 🧩 PART 7 — Closing (short & mature)

Add this 👇

```markdown
## Notes

This project focuses on understanding policy behavior through evaluation videos rather than achieving high task success. It serves as a foundation for further experimentation with longer training runs and GPU acceleration.
```

---

## ✅ Save & exit nano

Press:
```
CTRL + O → Enter
CTRL + X
```

---

## 🌟 What you now have

- A **real ML project README**
- Not flashy, but **serious**
- Perfect for GitHub, college, or future internships

---

### Next step options (pick one):

4️⃣ Create GitHub repo under **santhanuss** using `gh`  
5️⃣ Improve results (longer training / smaller model)  
6️⃣ Explain the videos *frame-by-frame* in simple language  

Just reply with the number 😼
