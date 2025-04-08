# ERC-24B3906
# The process for cleaning the given wave 
   Before we know how to clean the wave we need to know the process of wave trasmission
   >suppose say i want transfer a wave s(t),
>   >
>i cant directly tranfer it because its weak and can easily get attenuated
>
>so i need to modulate the wave with a wave of freq say Fc
>>now the modulated wave m(t) is
#   m(t)=(1 + s(t))cos(2 * pi * Fc * t)
>>after modulating while transfering the wave their ius some addition of noise sat n(t) in the path.
# the fianl wave we receive is m(t) + n(t)
#
#
#
From this we came to know that we have to fisrt find the modulating frequency and demopdulate the wave
#to find modulatring freq we need to perfoprm foreier teransformation to the wave

# 1.fourier transformation(fft)
#
from the fft functrion of numpy libraries in python i obtained the following graph

![fft](https://github.com/user-attachments/assets/231166a7-bb21-43dd-a757-64bbdcf45f45)

we can see that the the peak arew averaging towrad 10,000 so Fc=10,000
#
#2.demodulation and 3.filtering
#
after finding the Fc we can demodulate the wave by multiplying the given wave with cos(2 * pi * Fc * t).  
the demodulate wave is sent through filtering functions which filters the wave btw 300Hz to 4000hz which is human voice freq range which are plotted below
![Demodulated and Filtered signals](https://github.com/user-attachments/assets/880f5252-82d1-4fa4-b9fd-bc404cacdf57)
the final filtered sound wave is provided






