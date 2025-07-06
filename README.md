# Hotel Bookings Data Analysis

This project analyzes hotel booking data to uncover patterns and insights related to booking cancellations.
The main goal is to understand factors affecting cancellations and provide actionable recommendations to hotel management.

---

## Dataset Description

- Dataset Source: Kaggle (Hotel Bookings Dataset)
- Total Rows: 119,390
- Total Columns: 32

### Key Columns:
- `hotel`: Type of hotel (City Hotel, Resort Hotel)
- `is_canceled`: Booking cancellation status (0 = Not canceled, 1 = Canceled)
- `lead_time`: Number of days between booking and arrival
- `arrival_date_month`: Month of arrival
- `adults`, `children`, `babies`: Number of guests
- `customer_type`: Type of customer (Transient, Group, Contract, etc.)

---

## Data Cleaning

- Checked for missing values: None found.
- Converted `arrival_date_month` to ordered categories.
- Created `total_guests` = `adults` + `children` + `babies`

---

## Exploratory Data Analysis

### 1. Cancellation Rate (Overall)
- About 37% of bookings were canceled.

### 2. Cancellation by Hotel Type
- City Hotel: 41.73% cancellation rate
- Resort Hotel: 27.76% cancellation rate

### 3. Cancellation by Month
- June had the highest cancellation rate.

### 4. Cancellation vs Lead Time
- Longer lead times strongly correlate with higher cancellation rates.

### 5. Cancellation by Customer Type
- Transient customers cancel far more than Group or Contract types.

### 6. Cancellation by Total Guests
- Bookings with multiple guests (families/groups) cancel more than solo bookings.

---

## Key Insights and Recommendations

- Monitor long lead-time bookings closely.
- Offer incentives or stricter policies for Transient customers.
- Family bookings require flexible handling to reduce cancellations.
- June may require special attention due to high cancellation rates.
- City hotels should review policies or improve communication to reduce cancellations.

---

## How to Run

1. Clone this repository.
2. Download the dataset from [Kaggle](https://www.kaggle.com/jessemostipak/hotel-booking-demand)
3. Run the notebook file `hotel_analysis.ipynb` using Jupyter or Google Colab.

---

## Sample Visualization

*(Insert your visualizations here if desired)*

---

## License

This project is for educational purposes only.