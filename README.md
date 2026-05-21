# ecommerce-customer-segmentation-rfm
Data əsaslı müştəri seqmentasiyası: e-ticarət tranzaksiya məlumatları üzərində RFM (Recency, Frequency, Monetary) analizi.
# Pərakəndə Satış Data Analizi və Dashboard Layihəsi

## 📌 Layihə Haqqında
Bu layihədə e-ticarət tranzaksiya məlumatları üzərində RFM (Recency, Frequency, Monetary) analizi tətbiq edilərək müştərilər davranışlarına görə seqmentləşdirilir.

Məqsəd:
- Müştəri dəyərini ölçmək
- Ən aktiv və ən riskli müştəri qruplarını tapmaq
- Marketinq strategiyalarını data əsasında optimallaşdırmaq

## 🛠️ İstifadə Olunmuş Alətlər və Metodlar
* **Excel Funksiyaları:** XLOOKUP, IF, SUMIFS, Data Cleaning (Dublikatların silinməsi, boş xanaların doldurulması)
* **Data Qruplaşdırılması (Scoring Logic):** RFM metrikaları standart 1-5 ballıq şkala əvəzinə, müştəri davranışını daha dəqiq təsvir edən biznes yönümlü kateqoriyalara ayrılmışdır:
  * **Recency:** Active, Warm, At Risk, Churned və s.
  * **Frequency:** One-time, Occasional, Regular, Frequent, Loyal.
  * **Monetary:** Very Low Value, Low Value, Mid Value, High Value, Top Value.
  * **RFM Modelləşdirməsi:** Bu alt qrupların kombinasiyası yekun makro müştəri seqmentlərini (VIP, Loyal, Lost və s.) formalaşdırır.
* **Analiz:** Pivot Tables vasitəsilə KPI-ların hesablanması
* **Vizualizasiya:** Dinamik qrafiklər, Slicers və İnteraktiv Dashboard dizaynı

## 📊 Dashboard-dan Görüntü
Layihənin tam interaktiv dashboard görüntüsü aşağıdakı kimidir:

<img width="1872" height="810" alt="RFM Dashboard " src="https://github.com/user-attachments/assets/60b21257-2e55-46ee-a8e1-eba7a820621a" />

## 🧠 10 Kritik Biznes İnsight-ı və Strateji Həll Yolları 

### 1. Customer Activity Heatmap
<p align="center">
<img width="552" height="207" alt="image" src="https://github.com/user-attachments/assets/00b973c5-bb60-465f-8b28-21ada3f6fe5c" width="400">

### "Birdəfəlik Alıcı" (One-Time Buyer) Tələsi
* **Insight:** Customer Activity Heatmap əsasında, 625 "One-time" müştəri tamamilə itirilib (Churned), 929-u isə risk altındadır. Şirkət müştərini cəlb edə bilir, lakin ikinci alışa yönləndirməkdə uğursuz olur.
  
* **Action Plan:** İlk alışdan dərhal sonra başlayan 14 günlük aqressiv “Second Purchase Discount” kampaniyaları qurulmalıdır. Məqsəd müştərinin ikinci alış etmə ehtimalını artırmaq və “One-time” seqmentindən çıxmasını təmin etməkdir.

### 2. Monthly RFM Segment Performance
<p align="center">
<img width="916" height="207" alt="image" src="https://github.com/user-attachments/assets/a14d2fb3-9e57-4816-b922-5b2020f65f25" width="400">
  
### Qış Mövsümü vs. Yanvar Çöküşü (Seasonality Churn)
* **İnsight:** Aylıq trendlərdə Yeni Müştərilər Noyabr (13.98%) və Dekabrda (26.22%) zirvəyə çatır. Lakin İtirilmiş Müştərilər də məhz Yanvarda (31.42%) pik edir. Dördüncü rüb müştəriləri sistemdə qalmır.
* **Action Plan:** Noyabr/Dekabr aylarında sadəcə endirim deyil, gələcək ilin 1. rüb ayları üçün qüvvədə olacaq "Cashback" və ya "Xüsusi Endirim Kuponu"  tipli proqramlar təklif edilməlidir ki, müştəri Yanvarda geri dönsün.

### Stabil VIP Immuniteti
* **İnsight:** Aylıq trend cədvəlində VIP müştərilər (40-48% arası) ilin bütün aylarında stabilliyini qoruyur. Onlar mövsümi endirimlərə və ya bazar dalğalanmalarına reaksiya vermirlər.
* **Action Plan:** Bu sabit qrupdan oxşar profilli qruplar yaratmaq üçün istifadə edilməlidir.
  
### 3. Revenue Analysis 
<p align="center">
<img width="491" height="362" alt="image" src="https://github.com/user-attachments/assets/b70563c5-cd36-444f-b2c7-68aaa3bb6d08" width="400">

### Gəlir Konsentrasiyası Riski (Pareto Qanunu)
* **İnsight:** VIP (45%) və Loyal (21%) seqmentlər birlikdə ümumi biznes gəlirinin 66%-ni təmin edir. Portfelin kiçik bir kütlədən kəskin asılılığı biznes üçün yüksək riskdir.
* **Action Plan:** Bu qrup üçün ənənəvi xidmət üsulu ləğv edilməli, yerinə onlar üçün Fərdi Müştəri xidməti gətirilməlidir. Rəqiblərin bu qrupu hədəfləməsinə və onların digər hansısa bir səbəbdən biznesi təkr etmələrinə imkan verilməməlidir.

### 118 Milyonluq İtki
* **İnsight:** "Lost Customer" seqmentinin arxasında 118 Milyonluq bir gəlir keçmişi yatır. Bu baza sadəcə ölü data deyil, potensial qızıl mədənidir.
* **Action Plan:** Bu qrupa bizi niyə tərk etdiklərini öyrənmək üçün qısa sorğular və müqabilində yüksək dəyərli endirim kuponları (məsələn, 30% endirim) göndərilməlidir. Cəmi 5%-nin belə geri qaytarılması milyonlarla əlavə gəlir deməkdir.

### 4. Regional Segment Profile
<p align="center">
<img width="545" height="370" alt="image" src="https://github.com/user-attachments/assets/d9285979-e186-4c34-a4cd-7df604459d71" width="400">
  
### Birləşmiş Krallıq (UK) və İsveçrə Bazarında Qırmızı Siqnal
* **İnsight:** Coğrafi profildə UK bazarı böyük həcmə sahib olsa da, müştərilərin təqribən 45%-i "Lost" və ya "At Risk" qrupundadır. İsveçrədə isə itki nisbəti 60%-ə çatır.
* **Action Plan:** Bu regionlarda lokal logistika, gömrük problemləri və ya lokal rəqiblərin qiymət siyasəti dərhal araşdırılmalı, spesifik olaraq həmin ölkələr üçün "Xoş qayıtdın" kampaniyaları başladılmalıdır.

### 5. Customer Behaviour Matrix
<p align="center">
<img width="491" height="361" alt="image" src="https://github.com/user-attachments/assets/d69e40f5-a099-4857-aafb-ace1b2cfc353" width="400">

### "Top Value" seqmentinin Anomaliyası
* **İnsight:** Davranış Matrisində Top Value qrupu böyük fərqlə ayrılır: Ortalama alış miqdarı 20+, vahid qiymət 264+. Bu profil standart pərakəndə alıcı deyil, ehtimal ki, topdansatışçı və ya B2B müştərilərdir.
* **Action Plan:** Bu qrup üçün ümumi marketinq strategiyasından çıxararaq, onlara xüsusilə həcmə əsaslanan illik müqavilələr təklif edilməlidir.

### Orta Dəyər (Mid-Value) Sıxışması
* **İnsight:** Matrisdə "High Value" və "Mid Value" qrupları çox yaxın koordinatlarda (10-12 alış miqdarı) sıxışıb qalıblar. Onlar VIP səviyyəsinə keçid edə bilmirlər.
* **Action Plan:** Bu seqmentlərin Ortalama Sifariş Dəyərini (AOV) artırmaq üçün strateji satış üçün məhsul təklifləri alqoritmlərə daxil edilməlidir.


### 6. KPI Cards
<img width="1857" height="112" alt="image" src="https://github.com/user-attachments/assets/f7592351-6642-4713-8fb2-b21ca170b087" />

### Yüksək AOV (44K) vs Aşağı Aktivlik (41%) Paradoksu
* **İnsight:** 44K Ortalama Sifariş Dəyəri (AOV) olan bir biznesdə məhsullar çox bahalı və qərarvermə müddəti uzundur. Lakin aktiv müştəri nisbətinin yalnız 41% olması satış sonrası narazılığı göstərir.
* **Action Plan:** Yüksək biletli (High-ticket) satışlarda problem məhsulda deyil, çox güman ki, istifadəçi təcrübəsi və satış sonrası texniki xidmətdədir. "Customer Success" (Müştəri Uğuru) komandası yaradılmalı və məhsulun implementasiyası dövründə müştəriyə dəstək artırılmalıdır.

### "Müştəri Saxlama" (Retention) Böhranı 
* **İnsight:** 73% təkrar alış (Repeat Purchase) əladır, lakin 43% Churn (İtki) göstərir ki, sadəcə kiçik bir fanat qrupu davamlı alış edir, qalan kütlə isə sürətlə əriyir (Leaky bucket effect).
* **Action Plan:** Əldəki marketinq büdcəsinin böyük hissəsi yeni müştəri axtarışından (Acquisition) kəsilərək, mövcud bazanın saxlanılmasına (Retention) və Churn ehtimalı yüksək olanların erkən xəbərdarlıq sistemləri ilə (Predictive Analytics) qorunmasına yönəldilməlidir.

