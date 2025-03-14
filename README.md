# Module 5

**all-student** table before refactoring
![WhatsApp Image 2025-03-14 at 15 23 56_55d856d3](https://github.com/user-attachments/assets/2b8f0704-3b5c-426a-bba3-daf3c6b067e0)

**all-student-name** table before refactoring
![WhatsApp Image 2025-03-14 at 15 23 56_ddd50ba7](https://github.com/user-attachments/assets/3a2125b7-5966-4598-82e6-f1bc7b09678e)

**highest-gpa** table before refactoring
![WhatsApp Image 2025-03-14 at 15 23 56_144a766b](https://github.com/user-attachments/assets/a8018a1c-97e3-4553-8fc0-7c5979af5917)

**all-student** txt before refactoring
![WhatsApp Image 2025-03-14 at 16 27 16_eb081d47](https://github.com/user-attachments/assets/cf98cb8c-b9f5-4a49-a233-6773c5bff4d7)

**all-student-name** txt before refactoring
![WhatsApp Image 2025-03-14 at 16 27 15_144f239b](https://github.com/user-attachments/assets/408e2866-233d-4513-90d4-b9ef9358faa3)

**highest-gpa** txt before refactoring
![WhatsApp Image 2025-03-14 at 16 27 15_8a4ca9ab](https://github.com/user-attachments/assets/c6184182-9a54-41cf-80e9-fdd5e39e4d7e)

**all-student** table after refactoring
![WhatsApp Image 2025-03-14 at 16 56 43_818ae902](https://github.com/user-attachments/assets/79cb4853-3f47-4a81-b9c8-63df5034657c)

**all-student-name** table after refactoring
![WhatsApp Image 2025-03-14 at 16 56 44_60dc7e5a](https://github.com/user-attachments/assets/cce28e28-5110-4bf7-bd07-d578de825bb7)

**highest-gpa** table after refactoring
![WhatsApp Image 2025-03-14 at 16 56 44_dfb222f1](https://github.com/user-attachments/assets/cc592302-7875-4292-a407-372d53aca2f9)

**all-student** txt after refactoring
![WhatsApp Image 2025-03-14 at 16 59 10_d49cd02f](https://github.com/user-attachments/assets/a43c50f3-6b90-4762-91f7-62158dbdb947)

**all-student-name** txt after refactoring
![WhatsApp Image 2025-03-14 at 16 59 09_ec458a66](https://github.com/user-attachments/assets/c47b05eb-38f4-49fd-baf8-227479edbc9f)

**highest-gpa** txt after refactoring
![WhatsApp Image 2025-03-14 at 16 59 10_b05e8d79](https://github.com/user-attachments/assets/caed73ad-4f6f-4254-b923-0822737ac06d)

## Kesimpulan
Setelah optimisasi, proses profiling menjadi jauh lebih cepat. Dengan demikian, hal ini membuktikan keefektifan optimization dalam menciptakan kode yang lebih lancar dan cepat.

## Reflection
>1. What is the difference between the approach of performance testing with JMeter and profiling with IntelliJ Profiler in the context of optimizing application performance?
    Performance testing dengan JMeter berorientasi pada perspektif pengguna, yaitu dengan mensimulasikan beban eksternal untuk mengukur respons aplikasi seperti latency, throughput, dan error rate secara keseluruhan. Sebaliknya, IntelliJ Profiler fokus pada perspektif internal, yaitu menganalisis secara mendetail perilaku kode seperti konsumsi CPU, alokasi memori, serta waktu eksekusi per metode untuk menemukan bottleneck pada level kode. Kedua pendekatan ini berbeda namun saling melengkapi, memberikan gambaran menyeluruh tentang performa aplikasi.

>2. How does the profiling process help you in identifying and understanding the weak points in your application?
    Profiling memberikan gambaran yang detail tentang penggunaan sumber daya secara real-time, termasuk alokasi memori, penggunaan CPU, dan durasi eksekusi tiap method atau fungsi. Dengan visualisasi data ini, kita bisa langsung mengetahui secara akurat bagian kode mana yang inefisien, boros memori, atau terlalu sering dipanggil, sehingga optimasi dapat dilakukan secara tepat dan efisien.

>3. Do you think IntelliJ Profiler is effective in assisting you to analyze and identify bottlenecks in your application code?
    Ya, IntelliJ Profiler sangat efektif dalam menemukan dan menganalisis bottleneck di level kode aplikasi. Fitur visualisasi seperti flame graph mempermudah developer untuk memahami pola eksekusi, menemukan metode dengan konsumsi waktu tertinggi, serta memastikan optimasi yang dilakukan benar-benar efektif melalui fitur pembandingan performa sebelum dan sesudah perubahan.

>4. What are the main challenges you face when conducting performance testing and profiling, and how do you overcome these challenges?
    Tantangan utama adalah sulitnya membuat skenario pengujian realistis dan kompleksnya interpretasi data hasil profiling yang jumlahnya sangat besar. Cara mengatasinya adalah dengan merancang skenario pengujian seakurat mungkin, menggunakan container atau lingkungan isolasi seperti Docker untuk konsistensi hasil, dan melakukan iterasi pengujian berulang. Selain itu, pemahaman mendalam terhadap data profiling, visualisasi yang baik, serta penggunaan beberapa alat bantu lain juga sangat membantu dalam mengatasi tantangan tersebut.

>5. What are the main benefits you gain from using IntelliJ Profiler for profiling your application code?
    Manfaat utama IntelliJ Profiler adalah kemampuannya secara langsung menunjukkan titik-titik spesifik yang menjadi bottleneck pada aplikasi, seperti metode yang paling banyak menghabiskan waktu atau memori. Integrasi dengan IDE IntelliJ IDEA membuat proses profiling sangat efisien dan user-friendly. Fitur visualisasinya yang jelas juga mempercepat proses analisis serta membantu dalam memvalidasi efektivitas dari optimasi yang dilakukan.
    
>6. How do you handle situations where the results from profiling with IntelliJ Profiler are not entirely consistent with findings from performance testing using JMeter?
    Ketika terjadi perbedaan hasil antara IntelliJ Profiler dan JMeter, langkah pertama adalah memahami perbedaan perspektif dari kedua tools tersebut. IntelliJ lebih mengarah pada analisis internal kode, sedangkan JMeter melihat performa aplikasi secara keseluruhan dari sisi pengguna. Untuk mengatasi hal ini, dilakukan cross-verifikasi dengan menjalankan pengujian tambahan pada lingkungan isolasi, menganalisis faktor eksternal yang mungkin memengaruhi hasil, serta menggunakan alat pihak ketiga sebagai tambahan validasi agar didapatkan kesimpulan yang lebih akurat.

>7. What strategies do you implement in optimizing application code after analyzing results from performance testing and profiling? How do you ensure the changes you make do not affect the application's functionality?
    Setelah menganalisis hasil performance testing dan profiling, strategi yang biasanya diterapkan meliputi optimasi algoritma, memperbaiki penggunaan memori yang berlebihan, memanfaatkan fitur bahasa pemrograman (misalnya Java Stream API), dan mengurangi operasi yang tidak efisien seperti manipulasi String yang berat. Untuk memastikan optimasi ini tidak memengaruhi fungsionalitas, maka dilakukan kombinasi pengujian seperti unit test, integration test, dan continuous integration (CI). Pendekatan ini memastikan aplikasi tetap stabil dan berfungsi sesuai harapan setelah perubahan diterapkan.
