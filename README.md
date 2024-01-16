# Amplitude-Modulation-analysis
Amplitude Modulation using Wolfram Mathematica


It is possible to look at the theory of the generation of an amplitude-modulated signal in four steps: 
<br> I) Carrier signal 
<br>II) Modulating signal 
<br> III) Overall modulated signal for a single tone
<br> IV) Expansion to cover a typical audio signal

<br> The idea of ​​amplitude modulation is to transmit a low-frequency signal - voice or music - by modulating a high-frequency (carrier) signal, which is many times larger than the audible range and occupies a narrow frequency band in the radio air. 

```bash
 y(t) = [A + m(t)].C(t) 
```
![image](https://github.com/Chuggu12/Amplitude-Modulation-analysis/assets/108995664/8f5a66cf-25ef-4021-99df-d7beefccdfc7)

where A is the amplitude of the wave, C(t) is the carrier signal modulation, and m(t) is the modulating waveform can either be a single tone. This can be represented by a cosine waveform, or the modulating waveform could be a wide variety of frequencies - these can be represented by a series of cosine waveforms added together in a linear fashion,
where m(t) is  the modulating wave, and the modulating signal frequency in Hertz is equal to \[Omega]m / 2 \[Pi] is the phase of the signal at the start of the reference time, Both C and \[CurlyPhi] can be omitted to simplify the equation by changing C to "1" and \[CurlyPhi] to "0".

<br>In general form, a modulation process of a sinusoidal carrier wave may be described by the following equation:  m(t)= A(t). Cos(\[Omega]t +\[Phi](t))
Substituting in the individual relationships for the carrier and modulating signal, the overall signal becomes: y(t) = [A + Mcos(\[Omega]mt+\[CurlyPhi]].sin(\[Omega]ct)
                                                                                                                                                                
here we are taking the example of a wave having A as 1 and modulating waveform be Cos[x]  having a frequency as 1 and carrier wave as a function of cos having a frequency as 5.
```bash
 Cos(5x)*[Cos(x)+1]
```
![image](https://github.com/Chuggu12/Amplitude-Modulation-analysis/assets/108995664/0f2a5549-9668-4a23-8e01-c8e1a33c9dcb)


##Spectra Formation

We will do this by Fourier transformation on the sound wave equation breaking into Real and imaginary part of cosine  and sine wave formation, this theory can be used to break down a sound into a series of sinusoidal signals. These are linearly added to each other to form the audio spectrum of the modulating signal.

The spectrum of the modulating signal extends out either side from the carrier, one sideband is the mirror of the other, with the lowest frequencies closest to the carrier, and highest furthest away.
in the above diagram we see three terms can be seen which represent the carrier, and upper and lower sidebands:

<br>Carrier:     A . Cos (\[Omega]c +1)
<br>Upper sideband:     A . M/2 [ sin ((\[Omega]c + \[Omega]m) t + \[CurlyPhi])
<br>Lower sideband:     A . M/2 [ sin ((\[Omega]c - \[Omega]m) t - \[CurlyPhi])
![image](https://github.com/Chuggu12/Amplitude-Modulation-analysis/assets/108995664/6fffbaeb-bbef-484c-9bb3-be3366de2866)


where the  sidebands are separated from the carrier by a frequency equal to that of the tone. It can be seen that for a case where there is 100% modulation, i.e. M = 1, and where the carrier is not suppressed, i.e. A = 1, then the sidebands have half the value of the carrier, i.e. a quarter of the power each.


<br>Here we additionally obtained the Dirac delta function at the coordinate center \[LongDash] due to the presence of a constant component in the signal, which does not oscillate by definition \[LongDash], which allows us to consider it as a zero frequency.
![image](https://github.com/Chuggu12/Amplitude-Modulation-analysis/assets/108995664/ce948674-09f4-4a7e-94e6-bd0a2f5badf1)

In this, we do spectrum analysis by Fourier transformation forming spectral lines as upper and lower sidebands and also using reverse Fourier transformation to get the same A.M graphs and equation.

## License

[MIT](https://choosealicense.com/licenses/mit/)
<br> 💘 Ankit Anand

