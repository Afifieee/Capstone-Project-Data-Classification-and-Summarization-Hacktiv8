# Homeless Shelter Data Analysis
Analisis data homeless shelter menggunakan Colab + IBM Granite

## 📌 Project Overview
This project analyzes data from a local homeless shelter to uncover insights on program completion, substance abuse, income, and assistance types. The goal is to provide valuable recommendations for improving shelter programs.

## 📂 Dataset

- Dataset: https://www.kaggle.com/datasets/rezag7/homeless-dataset/data

     This dataset consists of data from a local homeless shelter that has gathered data on their homeless population seeking shelter.

     - CLIENT_KEY: This represents unique identifier of each client seeking shelter
     - AGE: This is the age of the client seeking shelter
     - GENDER: This is the gender of the client seeking shelter
     - VETERAN: This is an indicator to indicate if the client is a veteran or not
     - INCOME: This is the yearly income of the client seeking shelter
     - NIGHTS: This is the number of nights the client seeking shelter has stayed at the shelter
     - SUBSTANCEABUSE: This is an indicator to indicate if the client has substance abuse or not
     - COMPLETED: This is an indicator to indicate if the client has completed shelters program
     - PROBATION: This is an indicator to indicate if the client is on probation or not
     - ASSISTANCETYPE: This is the different types of assistance offered from the shelter
     - REQUIRED: This is an indicator to determin which assitance the client is requiring

## 🔍 Insights & Findings (berdasarkan output AI Granite)

**1.   Substance Abuse & Program Completion**
     
    Klien tanpa substance abuse punya tingkat completion 87.9%.
    
    Klien dengan substance abuse completion lebih rendah, hanya 67.6%.
     
    👉 Ada korelasi negatif, artinya masalah penyalahgunaan zat jadi hambatan keberhasilan program.

**2.   Income vs Nights**
     
    Korelasi antara INCOME dan NIGHTS = -0.053 (sangat lemah, hampir tidak ada).
     
    👉 Income bukan faktor dominan dalam lamanya tinggal di shelter, meskipun sedikit kecenderungan: yang berpenghasilan lebih tinggi tinggal lebih sedikit malam.

**3.   Veteran vs Non-Veteran**
      
    Dari dataset yang tersedia, tidak ditemukan bukti bahwa veteran atau non-veteran lebih banyak menyelesaikan program (jumlah completion = 0 untuk kedua kelompok).
      
    👉 Bisa jadi data incomplete/terlalu kecil untuk segment veteran → butuh data tambahan.

**4.   Assistance Type untuk Klien Berpenghasilan Rendah**

    Klien dengan INCOME = 0 paling banyak memilih bantuan tempassistance (bantuan sementara).
    
    👉 Bantuan jangka pendek paling krusial buat homeless tanpa penghasilan.

## 💡 Recommendations

**1.   Program pendampingan substance abuse**

    Perlu dibuat intervensi tambahan (rehabilitasi, konseling) agar tingkat keberhasilan klien dengan substance abuse bisa meningkat.

**2.   Fokus segmen veteran**

    Karena data veteran masih kosong, shelter perlu membangun tracking khusus veteran agar bisa menilai efektivitas program mereka.

**3.  Income-based support**

    Shelter bisa menyiapkan paket bantuan khusus klien 0 income (tempassistance + pelatihan kerja) supaya mereka bisa lebih cepat mandiri.

**4.  Dual shelter system**

    Mengembangkan shelter jadi hybrid: jangka pendek (emergency/temp assistance) dan jangka panjang (program pendampingan intensif).

## 🤖 AI Support
- Analysis supported by **IBM Granite Model (via Replicate API)** integrated in Google Colab.  
- AI assisted in generating insights, calculating correlations, and answering research questions automatically.
