# 📦 Shelf Arranger Web App

This is a **Streamlit web app** that arranges boxes on shelves optimally.

## 🚀 How to Deploy (Public Web App)

1. Go to [GitHub](https://github.com), create a **new repository** (public).
2. Upload these files:
   - `shelf_app.py`
   - `requirements.txt`
   - `README.md`
3. Go to [Streamlit Cloud](https://streamlit.io/cloud), sign in with GitHub.
4. Click **New app → Select your repo → Deploy**.
5. Done 🎉 You’ll get a public link like:

   ```
   https://your-username-shelf-arranger.streamlit.app
   ```

## 📊 Input Format

Upload an Excel file with 2 sheets:

### Sheet 1: Shelves
| Shelf_ID | Width | Height | Depth |
|----------|-------|--------|-------|
| Shelf_1  | 120   | 50     | 30    |
| Shelf_2  | 100   | 60     | 35    |

### Sheet 2: Boxes
| Box_ID | Width | Height | Depth | Quantity | AllowRotation | Priority |
|--------|-------|--------|-------|----------|---------------|----------|
| A      | 20    | 15     | 10    | 6        | TRUE          | 2        |
| B      | 25    | 20     | 12    | 4        | TRUE          | 1        |
| C      | 30    | 10     | 20    | 3        | FALSE         | 0        |

## 📥 Output

- Excel file (`shelf_arrangement.xlsx`) with:
  - **Placements** (coordinates per box)
  - **Unplaced** (boxes that didn’t fit)
- 3D visualization of shelves and boxes.
