Download Link: https://assignmentchef.com/product/solved-cfrm405-homework-3
<br>
<table width="646">

 <tbody>

  <tr>

   <td width="561"><strong>CFRM 405: Mathematical Methods for Quantitative Finance</strong>1. The Black-Scholes price for a European put option is</td>

   <td width="85"> </td>

  </tr>

  <tr>

   <td width="561"><em>P</em>(<em>S,t,K,T,r,q,σ</em>) = <em>Ke</em><sup>−<em>r</em>(<em>T</em>−<em>t</em>)</sup>Φ(−<em>d</em><sub>−</sub>) − <em>Se</em><sup>−<em>q</em>(<em>T</em>−<em>t</em>)</sup>Φ(−<em>d</em><sub>+</sub>)</td>

   <td width="85">(1)</td>

  </tr>

 </tbody>

</table>

where

and

Compute each of

by taking derivatives of (1). Verify that your answers are correct using put-call parity.

You can find expressions for <em>The Greeks </em>on pages 92 and 93 of the Stefanica text. Verify that your answer matches the expression for the put option and that put-call parity gives the expression for the call option. And as always, verify your calculations with Mathematica.

<strong>Example</strong>

Compute the vega of a European put option.

vega(

Lemma 3.15 states that <em>Ke</em><sup>−<em>r</em>(<em>T</em>−<em>t</em>)</sup><em>φ</em>(<em>d</em><sub>−</sub>) = <em>Se</em><sup>−<em>q</em>(<em>T</em>−<em>t</em>)</sup><em>φ</em>(<em>d</em><sub>+</sub>), thus

vega(

√                                 √

But <em>d</em><sub>− </sub>= <em>d</em><sub>+ </sub>− <em>σ               T </em>− <em>t </em>=⇒ <em>d</em><sub>+ </sub>− <em>d</em><sub>− </sub>= <em>σ         T </em>− <em>t</em>, thus

vega(

vega(

Check the result using put-call parity:

<em>P </em>= <em>C </em>− <em>Se</em>−<em>q</em>(<em>T</em>−<em>t</em>) + <em>Ke</em>−<em>r</em>(<em>T</em>−<em>t</em>)

vega(

The vega of a European put option is the same as the vega for a European call option.