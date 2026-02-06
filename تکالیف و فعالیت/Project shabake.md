Design and Implementation of an OFDM–MIMO Wireless Communication System

Abstract

Practical, project-based studies in wireless communications play a vital role in bridging theoretical concepts and real-world applications. This paper presents a complete project involving the design, simulation, and performance evaluation of a wireless communication system based on Orthogonal Frequency Division Multiplexing (OFDM) and Multiple-Input Multiple-Output (MIMO) technology. The primary objective of the project is to investigate the impact of channel conditions, noise, and antenna configurations on the Bit Error Rate (BER) and spectral efficiency of the system. Simulations are carried out in the MATLAB environment, and the results demonstrate that combining MIMO with OFDM significantly improves system performance.

Index Terms— Wireless communications, project-based study, OFDM, MIMO, simulation, MATLAB.


---

I. Introduction

With the rapid expansion of wireless communication systems, the demand for high data rate and reliable transmission has increased significantly. OFDM has emerged as the core modulation technique in 4G and 5G systems, while MIMO is one of the most effective methods for increasing channel capacity and link reliability.

This paper is designed as a project-based study that not only explains the theoretical foundations but also presents the practical steps required to implement a realistic wireless communication system. The proposed project is suitable for courses such as Digital Communications, Wireless Communications, and Cellular Communication Systems.


---

II. Problem Statement and Project Objectives

A. Problem Statement

Designing a wireless communication system capable of high-rate data transmission in the presence of noise and multipath fading is a fundamental challenge in communication engineering.

B. Project Objectives

Design an OFDM-based transmitter and receiver

Implement a 2×2 MIMO system

Model AWGN and Rayleigh fading channels

Compute and analyze the Bit Error Rate (BER)

Compare the performance of single-antenna OFDM and OFDM–MIMO systems



---

III. Proposed System Model

A. Overall System Structure

The proposed system consists of the following blocks:

1. Random data generation


2. QPSK modulation


3. OFDM processing (IFFT and Cyclic Prefix insertion)


4. Wireless channel (AWGN / Rayleigh)


5. OFDM receiver (CP removal and FFT)


6. Signal detection and data demodulation



B. MIMO Model

A 2×2 MIMO configuration with two transmit and two receive antennas is considered in this project. Zero-Forcing detection is employed at the receiver to separate the transmitted data streams.


---

IV. Implementation and Simulation

A. Simulation Environment

All simulations are conducted in the MATLAB environment. The main system parameters are summarized in Table I.

Table I – Simulation Parameters

Parameter	Value

Modulation	QPSK
Number of subcarriers	64
Cyclic Prefix length	16
MIMO configuration	2×2
Channel model	AWGN, Rayleigh


B. Implementation Steps

Generate random binary data

Map bits to QPSK symbols

Perform IFFT and add Cyclic Prefix

Apply channel effects and noise

Detect symbols and compute BER



---

V. Simulation Results and Analysis

Simulation results indicate that:

The OFDM–MIMO system outperforms the single-antenna OFDM system

The BER decreases as the Signal-to-Noise Ratio (SNR) increases

Rayleigh fading channels result in higher BER compared to AWGN channels


The BER versus SNR curves clearly demonstrate the advantages of employing MIMO technology.


---

VI. Proposed Project Extensions

The proposed project can be extended in several directions:

Employ higher-order modulation schemes (16-QAM, 64-QAM)

Implement channel coding techniques (Convolutional, LDPC)

Extend the system to Massive MIMO scenarios

Simulate 5G NR-based physical layer features

Implement the system using GNU Radio or USRP platforms



---

VII. Conclusion

This paper presented a complete project-based study on the design and simulation of an OFDM–MIMO wireless communication system. The obtained results confirm that the integration of OFDM and MIMO provides a robust and efficient solution for modern wireless communication systems. The proposed project serves as a solid foundation for advanced academic and research-oriented developments.


---

References

[1] J. G. Proakis, Digital Communications, McGraw-Hill, 2008.

[2] A. Goldsmith, Wireless Communications, Cambridge University Press, 2005.

[3] S. Haykin, Communication Systems, Wiley, 2014.

[4] T. S. Rappaport, Wireless Communications: Principles and Practice, Prentice Hall, 2002.



طراحی و پیاده‌سازی یک سیستم مخابرات بی‌سیم مبتنی بر OFDM و MIMO

چکیده

پروژه‌های عملی در حوزه مخابرات بی‌سیم نقش مهمی در درک عمیق مفاهیم تئوری و آماده‌سازی دانشجویان و پژوهشگران برای مسائل واقعی دارند. در این مقاله، یک پروژه‌ کامل شامل طراحی، شبیه‌سازی و ارزیابی عملکرد یک سیستم مخابرات بی‌سیم مبتنی بر OFDM و MIMO ارائه می‌شود. هدف اصلی پروژه، بررسی تأثیر کانال مخابراتی، نویز و پیکربندی آنتن‌ها بر نرخ خطای بیت (BER) و بازده طیفی سیستم است. شبیه‌سازی‌ها در محیط MATLAB انجام شده و نتایج نشان می‌دهند که استفاده از MIMO در کنار OFDM به‌طور قابل‌توجهی عملکرد سیستم را بهبود می‌بخشد.

واژگان کلیدی— مخابرات بی‌سیم، پروژه عملی، OFDM، MIMO، شبیه‌سازی، MATLAB.


---

I. مقدمه

با گسترش روزافزون سیستم‌های ارتباطی بی‌سیم، نیاز به طراحی و تحلیل سیستم‌هایی با نرخ داده بالا و قابلیت اطمینان مناسب بیش از پیش احساس می‌شود. فناوری OFDM به‌عنوان مدولاسیون اصلی در سیستم‌های 4G و 5G و فناوری MIMO به‌عنوان یکی از مهم‌ترین روش‌های افزایش ظرفیت کانال، نقش کلیدی در سیستم‌های مخابراتی مدرن دارند.

این مقاله یک پروژه‌محور طراحی شده است که علاوه بر تشریح مفاهیم تئوری، مراحل عملی پیاده‌سازی یک سیستم مخابراتی واقعی را نیز ارائه می‌دهد. این پروژه می‌تواند به‌عنوان پروژه درس مخابرات دیجیتال، مخابرات بی‌سیم، یا سیستم‌های سلولی مورد استفاده قرار گیرد.


---

II. تعریف مسئله و اهداف پروژه

A. تعریف مسئله

طراحی یک سیستم مخابرات بی‌سیم که قادر به ارسال داده با نرخ بالا در حضور نویز و کانال چندمسیره باشد، یکی از چالش‌های اصلی مهندسی مخابرات است.

B. اهداف پروژه

طراحی فرستنده و گیرنده OFDM

پیاده‌سازی سیستم MIMO با پیکربندی 2×2

مدل‌سازی کانال AWGN و Rayleigh

محاسبه و تحلیل نرخ خطای بیت (BER)

مقایسه عملکرد OFDM تک‌آنتنه و OFDM-MIMO



---

III. مدل سیستم پیشنهادی

A. ساختار کلی سیستم

سیستم پیشنهادی شامل بخش‌های زیر است:

1. تولید داده تصادفی


2. مدولاسیون QPSK


3. پیاده‌سازی OFDM (IFFT و افزودن Cyclic Prefix)


4. کانال مخابراتی (AWGN / Rayleigh)


5. گیرنده OFDM (حذف CP و FFT)


6. دمدولاسیون و آشکارسازی داده



B. مدل MIMO

در این پروژه از سیستم MIMO با دو آنتن فرستنده و دو آنتن گیرنده (2×2) استفاده شده است. برای آشکارسازی سیگنال از روش Zero-Forcing استفاده می‌شود.


---

IV. پیاده‌سازی و شبیه‌سازی

A. محیط شبیه‌سازی

تمامی شبیه‌سازی‌ها در محیط MATLAB انجام شده‌اند. پارامترهای اصلی سیستم در جدول زیر آمده است:

پارامتر	مقدار

مدولاسیون	QPSK
تعداد زیرحامل‌ها	64
طول Cyclic Prefix	16
پیکربندی MIMO	2×2
مدل کانال	AWGN، Rayleigh


B. مراحل پیاده‌سازی

تولید بیت‌های تصادفی

نگاشت بیت‌ها به سمبل‌های QPSK

انجام IFFT و افزودن CP

اعمال کانال و نویز

آشکارسازی و محاسبه BER



---

V. نتایج شبیه‌سازی و تحلیل

نتایج شبیه‌سازی نشان می‌دهد که:

سیستم OFDM-MIMO عملکرد بهتری نسبت به OFDM تک‌آنتنه دارد.

با افزایش SNR، نرخ خطای بیت کاهش می‌یابد.

کانال Rayleigh نسبت به AWGN باعث افزایش BER می‌شود.


نمودارهای BER بر حسب SNR به‌وضوح مزیت استفاده از MIMO را نشان می‌دهند.


---

VI. توسعه‌های پیشنهادی پروژه

این پروژه قابلیت توسعه در زمینه‌های زیر را دارد:

استفاده از مدولاسیون‌های مرتبه بالاتر (16-QAM، 64-QAM)

پیاده‌سازی کدینگ کانال (Convolutional، LDPC)

استفاده از Massive MIMO

شبیه‌سازی سناریوهای 5G NR

پیاده‌سازی در GNU Radio یا USRP



---

VII. نتیجه‌گیری

در این مقاله، یک پروژه‌ عملی و پروژه‌محور در حوزه مخابرات بی‌سیم ارائه شد که شامل طراحی و شبیه‌سازی سیستم OFDM-MIMO بود. نتایج به‌دست‌آمده نشان می‌دهند که ترکیب OFDM و MIMO راهکاری مؤثر برای افزایش قابلیت اطمینان و بازده سیستم‌های مخابراتی مدرن است. این پروژه می‌تواند مبنای مناسبی برای پروژه‌های پیشرفته‌تر و تحقیقات آتی باشد.


---

منابع

[1] J. G. Proakis, Digital Communications, McGraw-Hill, 2008.

[2] A. Goldsmith, Wireless Communications, Cambridge University Press, 2005.

[3] S. Haykin, Communication Systems, Wiley, 2014.

[4] T. S. Rappaport, Wireless Communications: Principles and Practice, Prentice Hall, 2002.
