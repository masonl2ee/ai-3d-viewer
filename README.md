# 🧠 AI 3D Viewer

An interactive 3D web viewer for `.asc` point cloud files, with AI-ready architecture for future shape detection and segmentation.

---

## 🚀 Features

- Upload and render `.asc` files as 3D point clouds
- Interact with the model: rotate, zoom, pan
- Lightweight and responsive UI built with Next.js and Three.js
- Modular structure for future AI integration (e.g., cylinder detection)

---

## 📁 Project Structure

```
ai-3d-viewer/
│
├── frontend/                     # Next.js frontend
│   ├── pages/                    # Main viewer page (index.tsx)
│   ├── components/               # Point cloud viewer & file upload
│   ├── public/pointcloud.json    # Sample converted .asc file
│   └── ...
│
├── backend/                      # AI inference or preprocessing backend
│   ├── convert_asc_to_json.py    # Converts .asc → .json for rendering
│   ├── model_inference.py        # Future AI model entry point
│   └── ...
│
├── data/                         # Raw .asc files
│   └── Measured_Data.asc
│
├── README.md
└── .gitignore
```

---

## 🛠️ Getting Started

### 1. Frontend Setup

```bash
cd frontend
npm install
npm run dev
```

Visit `http://localhost:3000` to launch the viewer.

### 2. Convert ASC to JSON

```bash
python backend/convert_asc_to_json.py
```

This will create a `pointcloud.json` file in the frontend's `public/` folder.

---

## 🔮 Upcoming Features

- [ ] Upload and preview any `.asc` file
- [ ] Highlight regions based on AI prediction
- [ ] Keyword-based geometry search (e.g., "cylinder")
- [ ] FastAPI backend for AI inference

---

## 🧠 Tech Stack

| Layer     | Tech                    |
|-----------|-------------------------|
| Frontend  | Next.js, React, Three.js |
| Backend   | Python, FastAPI (optional) |
| 3D Engine | react-three-fiber        |
| AI (TODO) | PyTorch, PointNet/PointNet++ |
