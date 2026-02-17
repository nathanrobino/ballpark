---
jupytext:
  text_representation:
    extension: .md
    format_name: myst
    format_version: 0.13
    jupytext_version: 1.19.1
kernelspec:
  display_name: Python 3
  language: python
  name: python3
---

+++ {"slideshow": {"slide_type": "slide"}}

<br><br><font size=10><b><center> Paper 2: "Population Aging and the Transmission of Monetary Policy to Consumption"  </center></b></font>
    <br><br>
    <font size=6><b><center> Arlene Wond (2015)</center></b></font>
    <br><br>
    <font size=5><b><center> Nino Kodua </center></b></font>
    <br><br>
    <font size=4><b><center> Johns Hopkins University </center></b></font>
    <br><br>
    <font size=4><b><center> February 16, 2020 </center></b></font>

+++ {"slideshow": {"slide_type": "slide"}}

# Overview

* **Research Question: What are the effects of demographic changes on the transmission of monetary policy to consumption?**
* **Part I: Empirical estimate**
    * **Age-specific consumption elasticities to interest rate**
        * **Consumption of young people is two-three times more responsive to interest rate shocks**
        * **Consumption elasticities decline with age**
    * **Consumption response driven by homeowners**
        * **refinance or new loans following interest rate decline**
* **Part II: Life-cycle model - partial equilibrium overlapping generations economy**
    * **Uninsurable labor income risk, life-cycle saving motive, fixed-rate mortgage structure**
    * **Fixed costs to adjust long-term assets**
        * **housing and fixed-rate mortgage**

+++ {"slideshow": {"slide_type": "slide"}}

# Household's maximization problem

* **Each period households choose**
    * **1. rent**
    * **2. continue owning a house & not adjust existing mortgage**
    * **3. adjust mortgage and housing stock**
* **Conditional on the adjustment, households choose**
    * **non-durable consumption, savings in bonds and mortgage debt**
<br>
<font size=3>
    <bold>
\begin{aligned}V_{j a t}\left(z_{j a t}\right)=\max \left\{V_{j a t}\left(z_{j a t}\right)^{\mathrm{rent}}, V_{j a t}\left(z_{j a t}\right)^{\mathrm{own} \& \text { no-adjust }}, V_{j a t}\left(z_{j a t}\right)^{\text {own } \& \text { adjust }}\right\}\end{aligned}      
    </bold>    
</font>   

<font size=3>
    <bold>
        \begin{aligned}
z_{j a t}=\left\{S_{t}, y_{j a t}, \operatorname{assets}_{j, a-1, t-1}\right\}
\end{aligned}      
    </bold>    
</font>   

* **$S_t$ - uncertainty from aggregate state variables**
* **$y_{j a t}$ - uncertainty from idiosyncratic labor income**

+++ {"slideshow": {"slide_type": "subslide"}}

# 1. Rent Case

<font size=3>
    <bold>
\begin{aligned}V_{j a t}\left(z_{j a t}\right)^{\mathrm{rent}}=\max _{c_{j a t}, h_{j a t}^{\mathrm{rat}}, s_{j a t}} \frac{\left(c_{j a t}^{\alpha} \cdot h_{j a t}^{1-\alpha}\right)^{1-\sigma}-1}{1-\sigma}+E_{j a t}\left[V_{j, a+1, t+1}\left(z_{j, a+1, t+1}\right)\right]\end{aligned}      
    </bold>    
</font> 

<font size=3>
    <bold>
        \begin{aligned} s.t. h_{j a t} &=h_{j a t}^{\text {rent }} \\ c_{j a t}+s_{j a t}+p_{t}^{r} h_{j a t}^{\text {rent }} &=y_{j a t}+(1-\delta) p_{t} h_{j, a-1, t-1}^{\text {own }}+\left(1+r_{t}\right) s_{j, a-1, t-1}-b_{j, a-1, t-1}\left(1+R_{j, a-1, t-1}\right) \\ h_{j a t}^{\text {own }} &=b_{j a t}=0 \\ s_{j a t} & \geq-\underline{s} \\ \log \left(y_{j a t}\right) &=\chi_{a}+\eta_{j a t}+\phi_{a}\left(y_{t} / y\right) \\ S_{t} &=A_{0}+A_{1} S_{t-1}+u_{t} \end{aligned}
          </bold>    
</font> 

+++ {"slideshow": {"slide_type": "subslide"}}

# 2. Own & No-adjust Case

<font size=3>
    <bold>
\begin{aligned}V_{j a t}\left(z_{j a t}\right)^{\text {own \& no-adjust }}=\max _{c_{j a t}, s_{j a t}} \frac{\left(c_{j a t}^{\alpha} \cdot h_{j a t}^{1-\alpha}\right)^{1-\sigma}-1}{1-\sigma}+E_{j a t}\left[V_{j, a+1, t+1}\left(z_{j, a+1, t+1}\right)\right]\end{aligned}      
    </bold>    
</font> 

<font size=3>
    <bold>
        \begin{aligned} s.t. h_{j a t} &=(1-\delta) h_{j, a, t-1}^{\mathrm{own}} \\ c_{j a t}+s_{j a t} &=y_{j a t}+\left(1+r_{t}\right) s_{j, a-1, t-1}-M_{j a t} \\ s_{j a t} & \geq-\underline{s} \\ \log \left(y_{j a t}\right) &=\chi_{a}+\eta_{j a t}+\phi_{a}\left(y_{t} / y\right) \\ S_{t} &=A_{0}+A_{1} S_{t-1}+u_{t} \end{aligned}
          </bold>    
</font> 

+++ {"slideshow": {"slide_type": "subslide"}}

# 3. Own & Adjust Case

<font size=3>
    <bold>
\begin{aligned}V_{j a t}\left(z_{j a t}\right)^{\text {own \& adjust }}=\max _{c_{j a t}, s_{j a t}, h_{j a t}^{\text {own }}, b_{j a t}} \frac{\left(c_{j a t}^{\alpha} \cdot h_{j a t}^{1-\alpha}\right)^{1-\sigma}-1}{1-\sigma}+E_{j a t}\left[V_{j, a+1, t+1}\left(z_{j, a+1, t+1}\right)\right] \end{aligned}      
    </bold>    
</font> 

<font size=3>
    <bold>
        \begin{aligned} s.t. h_{j a t} &=h_{j, a}^{\mathrm{own}} \\ b_{j a t} & \leq(1-\phi) p_{t} h_{j a t}^{\mathrm{own}} \\ c_{j a t}+s_{j a t}+p_{t} h_{j a t}^{\mathrm{own}}-b_{j a t}-F &=y_{j a t}+(1-\delta) p_{t} h_{j, a-1, t-1}^{\mathrm{own}}+\left(1+r_{t}\right) s_{j, a-1, t-1}-b_{j, a-1, t-1}\left(1+R_{j, a-1, t-1}\right) \\ s_{j a t} & \geq-\underline{s} \\ \log \left(y_{j a t}\right) &=\chi_{a}+\eta_{j a t}+\phi_{a}\left(y_{t} / y\right) \\ S_{t} &=A_{0}+A_{1} S_{t-1}+u_{t} \end{aligned}      
    </bold>    
</font> 

+++ {"slideshow": {"slide_type": "subslide"}}

# Retirement and Death

* **Upon death, agent bequasts total new wealth:**

<font size=3>
    <bold>
\begin{aligned}W_{j a t}=(1-\delta) p_{t} h_{j, a-1, t-1}^{\mathrm{own}}+\left(1+r_{t}\right) s_{j, a-1, t-1}
        \end{aligned}      
    </bold>    
</font> 

+++ {"slideshow": {"slide_type": "slide"}}

# Results

* **The refinancing and new lending channel** 
    * **the difference in the consumption responses of the young-old to interest rate shocks**
* **Aging population can significantly dampen the transmission of monetary policy**
