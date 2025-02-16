# E-commerce-Customer-Churn

### **Context**
Dalam era digital saat ini, industri e-commerce mengalami pertumbuhan yang pesat di seluruh dunia. Dengan semakin banyaknya platform e-commerce yang bermunculan, persaingan di pasar menjadi semakin ketat. Salah satu tantangan utama yang dihadapi oleh perusahaan e-commerce adalah customer churn,  Customer churn merujuk pada pelanggan yang berpotensi meninggalkan penyedia layanan dalam periode tertentu. Tujuan utama analisis churn adalah memprediksi pelanggan yang kemungkinan berpindah, mengidentifikasi penyebabnya, dan mengambil langkah untuk memperbaiki masalah. Pendekatan ini membantu memenuhi kebutuhan pelanggan agar tetap menggunakan layanan yang disediakan Wagh et al. (2024). 

---
### **Goals**
Tujuan dari analisis ini adalah untuk mengembangkan model prediksi berbasis machine learning yang dapat mengidentifikasi pelanggan berisiko churn, sehingga perusahaan e-commerce dapat menargetkan promosi lebih efisien kepada pelanggan yang tepat. Dengan memfokuskan penawaran pada pelanggan dengan potensi churn tinggi, perusahaan dapat mengurangi pemborosan anggaran dan kerugian pendapatan. Selain itu, dengan memahami faktor-faktor yang mempengaruhi churn, perusahaan dapat merancang promosi yang lebih relevan, meningkatkan loyalitas pelanggan, dan memperkuat hubungan dengan pelanggan yang ada. Tujuan ini diharapkan dapat meningkatkan retensi, mengurangi biaya akuisisi pelanggan baru, serta memperkuat daya saing perusahaan di pasar e-commerce.

---
### **Analytic Approach**
Pendekatan analitik ini dimulai dengan menganalisis data pelanggan untuk mengidentifikasi pola yang membedakan pelanggan yang berisiko churn dengan yang tidak. Berdasarkan analisis tersebut, model machine learning klasifikasi akan dibangun untuk memprediksi kemungkinan churn, yang memungkinkan perusahaan untuk mengarahkan strategi retensi secara lebih efisien dan tepat sasaran.

---
### **Metric Evaluation**
Dalam melakukan prediksi, terdapat dua jenis kesalahan yang mungkin terjadi:
1. **Kesalahan Tipe 1 (False Positive)**
    - Dampaknya: Perusahaan akan mengalami kerugian karena mengeluarkan biaya promosi untuk pelanggan yang tidak tepat sasaran.
3. **Kesalahan Tipe 2 (False Negative)**
    - Dampaknya: Perusahaan akan merugi karena pelanggan yang seharusnya diberi perhatian justru berhenti atau churn.
Target Prediksi:
- 0: Pelanggan tidak churn
- 1: Pelanggan churn

---
### **Confusion Metrix Term:**
- True Positive (TP): Pelanggan diprediksi akan churn dan memang benar-benar churn.
- False Positive (FP): Pelanggan diprediksi akan churn, tetapi sebenarnya tidak churn, yang menyebabkan kerugian operasional karena pengeluaran promosi yang tidak perlu.
- False Negative (FN): Pelanggan diprediksi tidak akan churn, tetapi sebenarnya churn, mengakibatkan kehilangan pendapatan karena tidak ada tindakan pencegahan.
- True Negative (TN): Pelanggan diprediksi tidak akan churn dan memang tidak churn, yang membantu perusahaan menghindari pemborosan sumber daya.
---
Penggunaan F2-Score sangat tepat untuk mengurangi False Negative (FN) dalam konteks prediksi churn, terutama untuk promosi yang bertujuan mencegah kehilangan pelanggan berisiko. Dalam model churn, mendeteksi pelanggan yang berpotensi churn lebih penting daripada menghindari promosi yang tidak tepat sasaran. F2-Score memberikan bobot lebih pada recall, meningkatkan sensitivitas model untuk mengidentifikasi pelanggan berisiko, meskipun bisa menambah False Positives (FP). Meskipun ada pengeluaran untuk promosi yang kurang efektif, manfaat utamanya adalah memastikan pelanggan yang berisiko churn tidak terlewatkan, yang sangat relevan di industri dengan tingkat churn tinggi atau yang bergantung pada retensi pelanggan.

---
Lihat cara kerja prediksi churn dengan mengunjungi platform ini: https://pengumpulancapston3-tlcdcrvmlfj3wdtmmgamtx.streamlit.app/
