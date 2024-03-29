# Calculate-LPB-and-RTB-in-Fiber-Optic
## This Project About How to Calculate LPB and RTB in Fibre Optic Using Python in Jupyter Notebook
<p>Link Power Budget (PLB) is an estimation of power requirements that is calculated to ensure that the level of receiving power is greater or equal to the threshold level (minimum power). LPB calculation is used to determine the maximum distance that can be achieved by the transmission system chosen, namely optical fiber. LPB calculations follow the ITU-T G.948 standard and also the regulations set by PT. Telkom Indonesia.The formula for calculating LPB is as follows:</p>
      <p align="center"><img src="https://render.githubusercontent.com/render/math?math=\alpha_T = 2\alpha_{c} %2B N_{s}\alpha_{s} %2B L\alpha_f %2B Ms" weight=1000 height=50></p>
with:
<l><img src="https://render.githubusercontent.com/render/math?math=\alpha_T= Total\\Attenuation"></l>
<l><img src="https://render.githubusercontent.com/render/math?math=\alpha_{c}= Attenuation\\of\\Connector"></l>
<l><img src="https://render.githubusercontent.com/render/math?math=N_{s}= Total\\of\\Splice\\Cable"></l>
<l><img src="https://render.githubusercontent.com/render/math?math=\alpha_{s}= Attenuation\\of\\Splice"></l>
<l><img src="https://render.githubusercontent.com/render/math?math=L= Distance"></l>
<l><img src="https://render.githubusercontent.com/render/math?math=\alpha_f= Attenuation\\of\\Fiber"></l>
<l><img src="https://render.githubusercontent.com/render/math?math=Ms= Margin\\System"></l>
<p>Rise time budget (RTB) is a method for determining the dispersion limits of a fiber optic communication system link which limits the bit rate of transmission capability. It is desirable that information sent from the transmitter can be read and received well by the receiver. The purpose of this method is to analyze whether the design results have good performance and are able to meet the desired channel capacity. The equation for calculating RTB is as follows:</p>
<p align="center"><img src="https://render.githubusercontent.com/render/math?math=\t_{sys}=\sqrt{t_{tx}^2 %2B t_{mat}^2 %2B t_{mod}^2 %2B t_{wg}^2 %2B t_{rx}^2}" weight=1000 height=50></p>
with:
<l><img src="https://render.githubusercontent.com/render/math?math=\t_{sys}= Total\\Dispertion"></l>
<l><img src="https://render.githubusercontent.com/render/math?math=\t_{tx}= Dispertion\\of\\Transmitter"></l>
<l><img src="https://render.githubusercontent.com/render/math?math=\t_{mat}= Dispertion\\of\\Material"></l>
<l><img src="https://render.githubusercontent.com/render/math?math=\t_{mod}= Dispertion\\of\\Mode"></l>
<l><img src="https://render.githubusercontent.com/render/math?math=\t_{wg}= Dispertion\\of\\Waveguide"></l>
<l><img src="https://render.githubusercontent.com/render/math?math=\t_{rx}= Dispertion\\of\\Receiver"></l>
<p align="center">
      <img src="https://user-images.githubusercontent.com/68779231/111249143-cf102180-863d-11eb-99b9-62da9c57d32c.PNG">
</p>
<p>In this case we will calculate LPB and RTB from Cilegon STO, Banten to Banjarmasin STO, South Kalimantan. We know that distance between them are 900 km. Communication System Point to Point for this case must be set gain from amplifier. There are some amplifier can set up in Communication System such as EDFA, RAMAN or SOA. We can set up for this case with EDFA(gain= 20dB). To set up an amplifier to the system, we must calculate how much amplifier with formula:</p>
<p align="center"><img src="https://render.githubusercontent.com/render/math?math=\alpha = G - M_{s}" weight=1000 height=50></p>
<p align="center"><img src="https://render.githubusercontent.com/render/math?math=L_{oa}=\frac{\alpha %2B \alpha_{s} %2B 2\alpha_{c}}{\alpha_{s} %2B \frac{\alpha_{s}}{100km}}" weight=1000 height=50></p>
