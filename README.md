# Apna-Safar-Tour-And-<!DOCTYPE html>
<html>
<head>
<title>Apna Safar Tour and Travels</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<style>
body { font-family: Arial; text-align: center; background: #000; color: gold; padding: 20px; }
button { padding: 12px; margin: 10px; width: 90%; font-size: 16px; }
input, select { padding: 10px; margin: 5px; width: 90%; }
</style>
</head>
<body>

<h2>Apna Safar Tour and Travels</h2>
<p>Local ₹15/km | Outstation ₹30/km</p>
<p>📞 9168031664</p>

<h3>Book Your Ride</h3>

<input type="text" id="name" placeholder="Your Name"><br>
<input type="number" id="mobile" placeholder="Mobile Number"><br>
<input type="number" id="distance" placeholder="Distance (KM)"><br>

<select id="type">
<option value="15">Local</option>
<option value="30">Outstation</option>
</select><br>

<button onclick="calculateFare()">Calculate Fare</button>

<h3 id="result"></h3>

<a href="tel:9168031664"><button>Call Now</button></a>
<a href="https://wa.me/919168031664"><button>Book on WhatsApp</button></a>

<script>
let bookingId = 1000;

function calculateFare() {
  let distance = document.getElementById("distance").value;
  let rate = document.getElementById("type").value;
  let fare = distance * rate;
  bookingId++;
  document.getElementById("result").innerHTML =
    "Booking ID: ASF" + bookingId + "<br>Total Fare: ₹" + fare;
}
</script>

</body>
</html><?xml version="1.0" encoding="utf-8"?>
<LinearLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    android:orientation="vertical"
    android:padding="24dp"
    android:gravity="center"
    android:layout_width="match_parent"
    android:layout_height="match_parent">

    <TextView
        android:text="Apna Safar Tour and Travels"
        android:textSize="22sp"
        android:textStyle="bold"
        android:layout_marginBottom="10dp"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"/>

    <TextView
        android:text="Maharashtra, Mumbai, Bhiwandi\nDeewan Shah Dargah Road, Golden Hotel"
        android:layout_marginBottom="20dp"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"/>

    <TextView
        android:text="Services:\n• Local Taxi\n• Intercity\n• All India\n• Airport Pickup/Drop\n• Rental"
        android:layout_marginBottom="30dp"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"/>

    <Button
        android:id="@+id/callBtn"
        android:text="Call Now"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"/>

    <Button
        android:id="@+id/whatsappBtn"
        android:text="Book on WhatsApp"
        android:layout_marginTop="15dp"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"/>

</LinearLayout>
