# Bhagwat Gita DataSet

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![GitHub Stars](https://img.shields.io/github/stars/username/Bhagwat-Gita-DataSet?style=social)](https://github.com/username/Bhagwat-Gita-DataSet)
[![GitHub Forks](https://img.shields.io/github/forks/username/Bhagwat-Gita-DataSet?style=social)](https://github.com/username/Bhagwat-Gita-DataSet)

## Overview

A Comprehensive And Structured DataSet Of The Sacred Bhagwat Gita, Containing All 720 Verses With Sanskrit Text, Hindi Translation, And English Translation. This DataSet Is Perfect For Spiritual Research, Natural Language Processing, Machine Learning Applications, And Educational Purposes.

## DataSet Structure

The DataSet Contains The Following Columns:

| Column Name | Description | Example |
|-------------|-------------|----------|
| **S.No.** | Serial Number Of The Verse | 1, 2, 3... |
| **Title** | Chapter Title In English | Arjuna's Vishada Yoga |
| **Chapter** | Chapter Number | Chapter 1, Chapter 2... |
| **Verse** | Verse Number | Verse 1.1, Verse 1.2... |
| **Sanskrit Anuvad** | Original Sanskrit Text | धृतराष्ट्र उवाच । धर्मक्षेत्रे कुरुक्षेत्रे... |
| **Hindi Anuvad** | Hindi Translation | धृतराष्ट्र बोले- हे संजय!... |
| **English Translation** | English Translation | Dhrtarashtra Asked Of Sanjaya... |

## DataSet Statistics

- **Total Verses**: 720
- **Total Chapters**: 18
- **Languages**: Sanskrit, Hindi, English
- **File Format**: CSV
- **File Size**: Approximately 2.5 MB
- **Encoding**: UTF-8

## Chapter Breakdown

| Chapter | Title | Verses Count |
|---------|-------|-------------|
| 1 | Arjuna's Vishada Yoga | 47 |
| 2 | Sankhya Yoga | 72 |
| 3 | Karma Yoga | 43 |
| 4 | Jnana Karma Sanyasa Yoga | 42 |
| 5 | Karma Sanyasa Yoga | 29 |
| 6 | Dhyana Yoga | 47 |
| 7 | Jnana Vijnana Yoga | 30 |
| 8 | Aksara Brahma Yoga | 28 |
| 9 | Raja Vidya Raja Guhya Yoga | 34 |
| 10 | Vibhuti Yoga | 42 |
| 11 | Viswarupa Darshana Yoga | 55 |
| 12 | Bhakti Yoga | 20 |
| 13 | Ksetra Ksetrajna Vibhaga Yoga | 35 |
| 14 | Gunatraya Vibhaga Yoga | 27 |
| 15 | Purushottama Yoga | 20 |
| 16 | Daivasura Sampad Vibhaga Yoga | 24 |
| 17 | Shraddhatraya Vibhaga Yoga | 28 |
| 18 | Moksha Sanyasa Yoga | 78 |

## Usage Examples

### Python

```python
import pandas as pd

# Load The DataSet
df = pd.read_csv('Main.csv')

# Display Basic Information
print(f"Total Verses: {len(df)}")
print(f"Total Chapters: {df['Chapter'].nunique()}")

# Get All Verses From Chapter 1
chapter_1 = df[df['Chapter'] == 'Chapter 1']
print(chapter_1[['Verse', 'English Translation']].head())

# Search For Specific Keywords
karma_verses = df[df['English Translation'].str.contains('karma', case=False, na=False)]
print(f"Verses Containing 'Karma': {len(karma_verses)}")
```

### R

```r
# Load The DataSet
data <- read.csv("Main.csv", stringsAsFactors = FALSE, encoding = "UTF-8")

# Display Basic Information
cat("Total Verses:", nrow(data), "\n")
cat("Total Chapters:", length(unique(data$Chapter)), "\n")

# Get Summary By Chapter
chapter_summary <- table(data$Chapter)
print(chapter_summary)
```

## Applications

### 🤖 Natural Language Processing
- **Text Analysis**: Sentiment Analysis Of Sacred Texts
- **Translation Models**: Training Multilingual Translation Systems
- **Text Classification**: Categorizing Verses By Themes
- **Named Entity Recognition**: Identifying Characters And Places

### 📊 Data Science & Machine Learning
- **Clustering Analysis**: Grouping Similar Verses
- **Topic Modeling**: Discovering Hidden Themes
- **Text Similarity**: Finding Related Verses
- **Recommendation Systems**: Suggesting Related Verses

### 🎓 Educational & Research
- **Comparative Studies**: Analyzing Different Translations
- **Linguistic Research**: Studying Sanskrit Language Patterns
- **Digital Humanities**: Creating Interactive Applications
- **Religious Studies**: Academic Research On Hindu Philosophy

### 📱 Application Development
- **Mobile Apps**: Daily Verse Applications
- **Web Platforms**: Online Bhagwat Gita Readers
- **Chatbots**: AI-Powered Spiritual Guidance
- **Search Engines**: Verse Discovery Platforms

## Installation & Setup

### Prerequisites
- Python 3.6+ Or R 3.5+
- Pandas (For Python) Or Base R (For R)
- Any Text Editor Or IDE

### Quick Start

1. **Clone The Repository**
   ```bash
   git clone https://github.com/username/Bhagwat-Gita-DataSet.git
   cd Bhagwat-Gita-DataSet
   ```

2. **Load The DataSet**
   ```python
   import pandas as pd
   df = pd.read_csv('Main.csv')
   ```

3. **Explore The Data**
   ```python
   print(df.head())
   print(df.info())
   ```

## Data Quality

- ✅ **Complete DataSet**: All 720 Verses Included
- ✅ **Accurate Translations**: Verified Sanskrit, Hindi, And English Texts
- ✅ **Consistent Formatting**: Standardized Column Names And Data Types
- ✅ **UTF-8 Encoding**: Proper Support For Sanskrit And Hindi Characters
- ✅ **No Missing Values**: Complete Data For All Fields

## Contributing

We Welcome Contributions To Improve This DataSet! Here's How You Can Help:

1. **Report Issues**: Found An Error? Please Create An Issue
2. **Suggest Improvements**: Have Ideas For Better Translations?
3. **Add Features**: Want To Add More Languages Or Annotations?
4. **Documentation**: Help Improve This README

### Contribution Guidelines

1. Fork The Repository
2. Create A Feature Branch (`git checkout -b Feature/AmazingFeature`)
3. Commit Your Changes (`git commit -m 'Add Some AmazingFeature'`)
4. Push To The Branch (`git push origin Feature/AmazingFeature`)
5. Open A Pull Request

## Citation

If You Use This DataSet In Your Research Or Applications, Please Cite:

```bibtex
@dataset{bhagwat_gita_dataset_2025,
  title={Bhagwat Gita DataSet: A Comprehensive Multilingual Collection},
  author={Durga AI Solutions},
  year={2025},
  url={https://github.com/username/Bhagwat-Gita-DataSet},
  note={Complete Sanskrit, Hindi, And English Translations Of All 720 Verses}
}
```

## License

This Project Is Licensed Under The MIT License - See The [LICENSE](LICENSE) File For Details.

## Acknowledgments

- 🙏 **Ancient Sages**: Who Composed This Timeless Scripture
- 📚 **Translators**: Who Made These Teachings Accessible
- 🤝 **Community**: Contributors Who Help Maintain Data Quality
- 💡 **Researchers**: Who Use This DataSet For Meaningful Applications

## Contact

For Questions, Suggestions, Or Collaborations:

- **Email**: contact@durgaaisolutions.com
- **GitHub**: [Create An Issue](https://github.com/username/Bhagwat-Gita-DataSet/issues)
- **Website**: https://durgaaisolutions.com

## Disclaimer

This DataSet Is Created For Educational And Research Purposes. While Every Effort Has Been Made To Ensure Accuracy, Please Consult Original Sanskrit Texts And Scholarly Translations For Authoritative References.

---

**🕉️ May This DataSet Serve The Purpose Of Spreading The Eternal Wisdom Of The Bhagwat Gita To Researchers, Developers, And Spiritual Seekers Worldwide! 🕉️**