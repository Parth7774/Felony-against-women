<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UT-7">
 
  
<body>

  <h1>🎬 Felony Against Women: Hate & Offensive Speech Detection from Media</h1>
  <p>This project investigates hate and offensive speech, especially targeting women, by analyzing subtitles from popular movies and comments from social media platforms.</p>

  <div class="structure">
    <h2>📂 Dataset Structure</h2>
    <pre>
FELONY-AGAINST-WOMEN/
├── data/
│   ├── Movies/
│   │   ├── for_training/
│   │   └── raw/
│   ├── fox_news.csv
│   ├── twitter.csv
│   └── all_movies.csv
├── data_preprocess/
│   ├── CSV_combined_dialogs/
│   ├── mturk_format/
│   ├── SRT/
│   └── SRT_TO_CSV/
├── models/
├── combining_utterances.ipynb
├── convert_movies_to_mturk_format.ipynb
├── Inter_Annotator_Agreement.ipynb
└── SRT_to_CSV_preprocess_.ipynb
    </pre>
  </div>

  <div class="dataset">
    <h2>📊 Datasets Used</h2>

    <h3>🐦 Twitter Dataset</h3>
    <ul>
      <li><strong>Source:</strong> <a href="https://github.com/t-davidson/hate-speech-and-offensive-language/">Davidson et al. GitHub</a></li>
      <li><strong>Size:</strong> 24,802 tweets</li>
      <li><strong>Labels:</strong> Hate Speech, Offensive, Neither</li>
      <li><strong>Note:</strong> Removed 204 duplicate tweets for better quality.</li>
    </ul>

    <h3>📰 Fox News Comments</h3>
    <ul>
      <li><strong>Source:</strong> <a href="https://github.com/sjtuprog/fox-news-comments">SJTUPROG GitHub</a></li>
      <li><strong>Size:</strong> 1,528 comments from 10 threads (2016)</li>
      <li><strong>Labels:</strong> Hate Speech, Normal</li>
      <li><strong>Note:</strong> Cleaned 13 duplicates and 2 empty entries.</li>
    </ul>

    <h3>🎞️ Movie Subtitles Dataset</h3>
    <ul>
      <li>Extracted from 6 IMDb-tagged films</li>
      <li>Annotated using Amazon MTurk</li>
      <li><strong>Hate Speech Focused:</strong> BlacKkKlansman (2018)</li>
      <li><strong>Racism Depicted:</strong> Django Unchained, American History X, Pulp Fiction</li>
      <li><strong>Friendship-based (for contrast):</strong> South Park, The Wolf of Wall Street</li>
      <li>Combined data available in <code>all_movies.csv</code></li>
    </ul>
  </div>

  <div class="video">
    <h2>📹 Project Video Demo</h2>
    <p><a href="https://drive.google.com/file/d/1Y1AvQL6LB0NvtbL70O6D-Vv8kPfHwhsl/view?usp=sharing" target="_blank">▶️ Click to Watch</a></p>
  </div>

  <div class="purpose">
    <h2>💡 Purpose</h2>
    <ul>
      <li>Analyze harmful speech in movies and social media</li>
      <li>Train detection models using rich and diverse datasets</li>
      <li>Expose gender-specific offensive language patterns</li>
    </ul>
  </div>

  <div class="tech">
    <h2>🛠️ Tools & Technologies</h2>
    <ul>
      <li>Python (Jupyter Notebooks)</li>
      <li>Pandas, NumPy, Scikit-learn</li>
      <li>Amazon MTurk</li>
      <li>Rainbow CSV Extension (VS Code)</li>
    </ul>
  </div>

  <div class="contribute">
    <h2>🤝 Contributions</h2>

