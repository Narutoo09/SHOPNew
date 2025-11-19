# Farm & Filter Customer Analytics Dashboard 🌿

An interactive Streamlit dashboard for analyzing customer data and validating the business model for **Farm & Filter** - a modern organic cafe, community wellness hub, and remote-work-friendly space.

## 📋 Project Overview

This dashboard provides comprehensive data-driven insights for the Farm & Filter business concept, featuring:

- **Customer Demographics Analysis**: Understand your target audience by age, income, and location
- **Health & Organic Preferences**: Validate the organic cafe concept with spending patterns
- **Workspace Analytics**: Analyze remote worker needs and workspace requirements
- **Customer Priorities**: Identify what matters most to your customers
- **3D Golden Segment Visualization**: Discover high-value customer profiles

## 🎯 Features

### Interactive Filters
- Age group selection
- Income level filtering
- Remote work frequency
- Health consciousness score range

### Key Metrics Dashboard
- Total customers
- Average spending per visit
- High interest customer count
- Average health consciousness score
- Remote worker statistics

### Visualizations
1. **Demographics & Spending**: Age-based spending patterns and income-frequency heatmaps
2. **Health Validation**: Organic importance vs. spending correlation
3. **Menu Preferences**: Top menu items by customer preference
4. **Workspace Insights**: Remote work distribution and workspace needs
5. **Priority Rankings**: Customer decision factors
6. **Location Strategy**: Distance-based spending and frequency analysis
7. **3D Golden Segment**: Multi-dimensional customer segmentation

## 🚀 Getting Started

### Prerequisites
- Python 3.8 or higher
- pip (Python package manager)

### Installation

1. **Clone or download this repository**
   ```bash
   git clone <your-repository-url>
   cd farm-filter-dashboard
   ```

2. **Install required packages**
   ```bash
   pip install -r requirements.txt
   ```

3. **Ensure data file is present**
   - Make sure `farm_filter_customer_data.csv` is in the same directory as `app.py`

4. **Run the Streamlit app**
   ```bash
   streamlit run app.py
   ```

5. **Open your browser**
   - The app will automatically open at `http://localhost:8501`
   - If not, manually navigate to the URL shown in the terminal

## 📦 Files Included

```
farm-filter-dashboard/
│
├── app.py                           # Main Streamlit application
├── farm_filter_customer_data.csv    # Customer dataset (600 profiles)
├── requirements.txt                 # Python dependencies
└── README.md                        # This file
```

## 🌐 Deployment to Streamlit Cloud

### Step 1: Create a GitHub Repository

1. Go to [GitHub](https://github.com) and sign in
2. Click **New Repository**
3. Name it (e.g., `farm-filter-dashboard`)
4. Make it **Public**
5. Click **Create Repository**

### Step 2: Upload Files to GitHub

**Option A: Via Web Interface (Easiest)**
1. On your repository page, click **uploading an existing file**
2. Drag and drop all files:
   - `app.py`
   - `farm_filter_customer_data.csv`
   - `requirements.txt`
   - `README.md`
3. Scroll down and click **Commit changes**

**Option B: Via Git Command Line**
```bash
git init
git add .
git commit -m "Initial commit"
git remote add origin <your-repo-url>
git branch -M main
git push -u origin main
```

### Step 3: Deploy on Streamlit Community Cloud

1. Go to [share.streamlit.io](https://share.streamlit.io)
2. Sign in with your GitHub account
3. Click **New app**
4. Select your repository: `<username>/farm-filter-dashboard`
5. Set the main file path: `app.py`
6. Click **Deploy**
7. Wait 2-5 minutes for deployment
8. Your app will be live at: `https://<username>-farm-filter-dashboard-<hash>.streamlit.app`

## 📊 Data Description

The dashboard uses synthetic data representing 600 potential customers with the following attributes:

### Demographics
- Age (18-64)
- Age Group (5 categories)
- Annual Household Income (5 brackets)
- Distance from Location (5 ranges)

### Behavioral
- Dining Out Frequency (4 levels)
- Remote Work Frequency (4 levels)

### Psychographic (1-5 scale)
- Health Consciousness Score
- Importance of Organic
- Workspace Need Score
- Interest in Farm & Filter

### Spending & Preferences
- Average Spending Per Visit ($)
- Customer Priorities (Taste, Price, Location, Ambiance)
- Menu Item Preferences (Binary flags)

## 🎨 Dashboard Sections

### 1. Key Performance Indicators
Quick overview metrics displayed at the top

### 2. Customer Demographics & Spending Patterns
- Bar chart: Average spending by age group
- Heatmap: Income vs. dining frequency

### 3. Health Consciousness & Organic Preferences
- Line chart: Organic importance vs. spending
- Bar chart: Top menu item preferences

### 4. Workspace & Remote Work Insights
- Pie chart: Remote work distribution
- Line chart: Workspace needs vs. spending

### 5. Customer Priorities & Location Strategy
- Horizontal bar: Priority rankings
- Dual-axis: Distance analysis

### 6. Golden Segment Analysis
- 3D scatter plot: Health × Workspace × Spending × Interest

### 7. Data Table & Export
- Filterable data table
- CSV download option

## 🛠️ Customization

### Modify Color Schemes
Edit the `color_continuous_scale` in Plotly charts:
```python
color_continuous_scale='Greens'  # Change to 'Blues', 'Reds', etc.
```

### Add New Filters
In the sidebar section, add:
```python
new_filter = st.sidebar.selectbox("Filter Name", options)
```

### Add New Visualizations
Use Plotly Express or Graph Objects:
```python
fig = px.bar(data, x='column1', y='column2')
st.plotly_chart(fig, use_container_width=True)
```

## 📚 Technologies Used

- **Streamlit**: Web application framework
- **Pandas**: Data manipulation and analysis
- **NumPy**: Numerical computing
- **Plotly**: Interactive visualizations

## 🤝 Contributing

This is an academic project. For suggestions or improvements:
1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## 📝 License

This project is created for educational purposes as part of a Data Analytics course assignment.

## 👤 Author

**Amanpreet Singh** (MS25LMM024)
- Project: Farm & Filter Business Validation
- Course: Data Analytics - MGB
- Assignment: Project Based Learning - Individual and Group Project

## 🙏 Acknowledgments

- Data generated synthetically for educational purposes
- Dashboard design inspired by modern data visualization best practices
- Built as part of MGB Data Analytics course

## 📞 Support

For issues or questions:
1. Check the [Streamlit Documentation](https://docs.streamlit.io)
2. Review the [Plotly Documentation](https://plotly.com/python/)
3. Open an issue on GitHub

## 🔄 Version History

- **v1.0.0** (November 2025)
  - Initial release
  - Full dashboard with 8+ visualizations
  - Interactive filtering capabilities
  - Data export functionality

---

**Happy Analyzing! 📊🌿**
