# depression-PMBFN
This is the details about the PMBFN model architecture in the "Parallel Multi-Scale Bridge Fusion Network for Audio-Visual Automatic Depression Assessment" paper.

We have provided specific information about the core components of PMBFN in the following table.

<table class="MsoTableGrid" border="1" cellspacing="0" cellpadding="0" width="926" style="width:694.6pt;border-collapse:collapse;border:none;mso-border-alt:solid windowtext .5pt;
 mso-yfti-tbllook:1184;mso-padding-alt:0cm 5.4pt 0cm 5.4pt">
 <tbody><tr style="mso-yfti-irow:0;mso-yfti-firstrow:yes;height:17.45pt">
  <td width="218" valign="top" style="width:163.5pt;border:solid windowtext 1.0pt;
  mso-border-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt;height:17.45pt">
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">Module<o:p></o:p></span></p>
  </td>
  <td width="349" valign="top" style="width:261.8pt;border:solid windowtext 1.0pt;
  border-left:none;mso-border-left-alt:solid windowtext .5pt;mso-border-alt:
  solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt;height:17.45pt">
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">Module Details<o:p></o:p></span></p>
  </td>
  <td width="113" valign="top" style="width:3.0cm;border:solid windowtext 1.0pt;
  border-left:none;mso-border-left-alt:solid windowtext .5pt;mso-border-alt:
  solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt;height:17.45pt">
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">Numbers<o:p></o:p></span></p>
  </td>
  <td width="246" valign="top" style="width:184.25pt;border:solid windowtext 1.0pt;
  border-left:none;mso-border-left-alt:solid windowtext .5pt;mso-border-alt:
  solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt;height:17.45pt">
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">Output Size<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style="mso-yfti-irow:1;height:64.65pt">
  <td width="218" style="width:163.5pt;border:solid windowtext 1.0pt;border-top:
  none;mso-border-top-alt:solid windowtext .5pt;mso-border-alt:solid windowtext .5pt;
  padding:0cm 5.4pt 0cm 5.4pt;height:64.65pt">
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">Spatial Encoder
  x2<o:p></o:p></span></p>
  </td>
  <td width="349" style="width:261.8pt;border-top:none;border-left:none;
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt;height:64.65pt">
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">Residual Con1d 1
  x 1<o:p></o:p></span></p>
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">A: 128</span><span style="font-size:12.0pt;mso-ascii-font-family:&quot;Times New Roman&quot;;mso-hansi-font-family:
  &quot;Times New Roman&quot;;mso-bidi-font-family:&quot;Times New Roman&quot;">、</span><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">64</span><span style="font-size:12.0pt;mso-ascii-font-family:&quot;Times New Roman&quot;;mso-hansi-font-family:
  &quot;Times New Roman&quot;;mso-bidi-font-family:&quot;Times New Roman&quot;">、</span><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">128
  kernels<o:p></o:p></span></p>
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">V:<span style="mso-spacerun:yes">&nbsp; </span>64</span><span style="font-size:12.0pt;
  mso-ascii-font-family:&quot;Times New Roman&quot;;mso-hansi-font-family:&quot;Times New Roman&quot;;
  mso-bidi-font-family:&quot;Times New Roman&quot;">、</span><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">32</span><span style="font-size:12.0pt;mso-ascii-font-family:&quot;Times New Roman&quot;;mso-hansi-font-family:
  &quot;Times New Roman&quot;;mso-bidi-font-family:&quot;Times New Roman&quot;">、</span><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">64
  kernels<o:p></o:p></span></p>
  </td>
  <td width="113" style="width:3.0cm;border-top:none;border-left:none;border-bottom:
  solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;mso-border-top-alt:
  solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;mso-border-alt:
  solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt;height:64.65pt">
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">3<o:p></o:p></span></p>
  </td>
  <td width="246" style="width:184.25pt;border-top:none;border-left:none;
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt;height:64.65pt">
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">A: 9 x 200 x 128<o:p></o:p></span></p>
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">V: 25 x 200 x 64<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style="mso-yfti-irow:2;height:18.1pt">
  <td width="218" rowspan="7" style="width:163.5pt;border:solid windowtext 1.0pt;
  border-top:none;mso-border-top-alt:solid windowtext .5pt;mso-border-alt:solid windowtext .5pt;
  padding:0cm 5.4pt 0cm 5.4pt;height:18.1pt">
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">PMDCL-<span class="GramE">A <span style="mso-spacerun:yes">&nbsp;</span>x</span>4<o:p></o:p></span></p>
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">PMDCL-<span class="GramE">V<span style="mso-spacerun:yes">&nbsp; </span>x</span>4<o:p></o:p></span></p>
  </td>
  <td width="349" valign="top" style="width:261.8pt;border-top:none;border-left:
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt;height:18.1pt">
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">Conv1d 1 x 1 stride=1<o:p></o:p></span></p>
  </td>
  <td width="113" valign="top" style="width:3.0cm;border-top:none;border-left:none;
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt;height:18.1pt">
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">4<o:p></o:p></span></p>
  </td>
  <td width="246" rowspan="7" style="width:184.25pt;border-top:none;border-left:
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt;height:18.1pt">
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">A: 9 x T A x 128<o:p></o:p></span></p>
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">V: 25 x T V x 64<o:p></o:p></span></p>
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">TA = 200, 100,
  50, 25<o:p></o:p></span></p>
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">TV = 200, 100,
  50, 25<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style="mso-yfti-irow:3;height:17.75pt">
  <td width="349" valign="top" style="width:261.8pt;border-top:none;border-left:
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt;height:17.75pt">
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">Conv1d 1 x 3 stride=1<o:p></o:p></span></p>
  </td>
  <td width="113" valign="top" style="width:3.0cm;border-top:none;border-left:none;
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt;height:17.75pt">
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">1<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style="mso-yfti-irow:4;height:17.75pt">
  <td width="349" valign="top" style="width:261.8pt;border-top:none;border-left:
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt;height:17.75pt">
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">Conv1d 1 x 5 stride=1<o:p></o:p></span></p>
  </td>
  <td width="113" valign="top" style="width:3.0cm;border-top:none;border-left:none;
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt;height:17.75pt">
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">1<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style="mso-yfti-irow:5;height:17.75pt">
  <td width="349" valign="top" style="width:261.8pt;border-top:none;border-left:
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt;height:17.75pt">
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">Dilated Conv1d 1
  x 3 dilated rate=1<o:p></o:p></span></p>
  </td>
  <td width="113" valign="top" style="width:3.0cm;border-top:none;border-left:none;
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt;height:17.75pt">
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">1<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style="mso-yfti-irow:6;height:17.75pt">
  <td width="349" valign="top" style="width:261.8pt;border-top:none;border-left:
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt;height:17.75pt">
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">Dilated Conv1d 1
  x 3 dilated rate=3<o:p></o:p></span></p>
  </td>
  <td width="113" valign="top" style="width:3.0cm;border-top:none;border-left:none;
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt;height:17.75pt">
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">1<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style="mso-yfti-irow:7;height:17.75pt">
  <td width="349" valign="top" style="width:261.8pt;border-top:none;border-left:
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt;height:17.75pt">
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">Dilated Conv1d 1
  x 3 dilated rate=5<o:p></o:p></span></p>
  </td>
  <td width="113" valign="top" style="width:3.0cm;border-top:none;border-left:none;
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt;height:17.75pt">
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">1<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style="mso-yfti-irow:8;height:17.75pt">
  <td width="349" valign="top" style="width:261.8pt;border-top:none;border-left:
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt;height:17.75pt">
  <p class="MsoNormal" align="center" style="text-align:center"><span class="GramE"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">LSTM <span style="mso-spacerun:yes">&nbsp;</span>A</span></span><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">: 128 Nodes <span style="mso-spacerun:yes">&nbsp;</span>V:64 Nodes<o:p></o:p></span></p>
  </td>
  <td width="113" valign="top" style="width:3.0cm;border-top:none;border-left:none;
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt;height:17.75pt">
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">2<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style="mso-yfti-irow:9;height:69.95pt">
  <td width="218" style="width:163.5pt;border:solid windowtext 1.0pt;border-top:
  none;mso-border-top-alt:solid windowtext .5pt;mso-border-alt:solid windowtext .5pt;
  padding:0cm 5.4pt 0cm 5.4pt;height:69.95pt">
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">Pooling-<span class="GramE">A <span style="mso-spacerun:yes">&nbsp;</span>x</span>3<o:p></o:p></span></p>
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">Pooling-<span class="GramE">V <span style="mso-spacerun:yes">&nbsp;</span>x</span>3<o:p></o:p></span></p>
  </td>
  <td width="349" style="width:261.8pt;border-top:none;border-left:none;
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt;height:69.95pt">
  <p class="MsoNormal" align="center" style="text-align:center"><span class="SpellE"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">Maxpooling</span></span><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif"> 1 x
  2 stride=2<o:p></o:p></span></p>
  </td>
  <td width="113" style="width:3.0cm;border-top:none;border-left:none;border-bottom:
  solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;mso-border-top-alt:
  solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;mso-border-alt:
  solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt;height:69.95pt">
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">1<o:p></o:p></span></p>
  </td>
  <td width="246" valign="top" style="width:184.25pt;border-top:none;border-left:
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt;height:69.95pt">
  <p class="MsoNormal" align="center" style="margin-left:12.0pt;text-align:center;
  text-indent:-12.0pt;mso-char-indent-count:-1.0"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">A: 9 x T A x 128<o:p></o:p></span></p>
  <p class="MsoNormal" align="center" style="margin-left:12.0pt;text-align:center;
  text-indent:-12.0pt;mso-char-indent-count:-1.0"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">TA=100, 50, 25<o:p></o:p></span></p>
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">V: 25 x T V x 64<o:p></o:p></span></p>
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">TV=100, 50, 25<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style="mso-yfti-irow:10;height:17.75pt">
  <td width="218" rowspan="4" style="width:163.5pt;border:solid windowtext 1.0pt;
  border-top:none;mso-border-top-alt:solid windowtext .5pt;mso-border-alt:solid windowtext .5pt;
  padding:0cm 5.4pt 0cm 5.4pt;height:17.75pt">
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">STAP-<span class="GramE">A<span style="mso-spacerun:yes">&nbsp; </span>x</span>4<o:p></o:p></span></p>
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">STAP-<span class="GramE">V<span style="mso-spacerun:yes">&nbsp; </span>x</span>4<o:p></o:p></span></p>
  </td>
  <td width="349" valign="top" style="width:261.8pt;border-top:none;border-left:
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt;height:17.75pt">
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">AdaptiveAvgPool2d<o:p></o:p></span></p>
  </td>
  <td width="113" valign="top" style="width:3.0cm;border-top:none;border-left:none;
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt;height:17.75pt">
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">1<o:p></o:p></span></p>
  </td>
  <td width="246" rowspan="4" valign="top" style="width:184.25pt;border-top:none;
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt;height:17.75pt">
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">A</span><span style="font-size:12.0pt;mso-ascii-font-family:&quot;Times New Roman&quot;;mso-hansi-font-family:
  &quot;Times New Roman&quot;;mso-bidi-font-family:&quot;Times New Roman&quot;">：</span><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">TA x
  128<o:p></o:p></span></p>
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">V:<span style="mso-spacerun:yes">&nbsp; </span>TV x 64<o:p></o:p></span></p>
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">TA = 200, 100,
  50, 25<o:p></o:p></span></p>
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">TV = 200, 100,
  50, 25<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style="mso-yfti-irow:11;height:17.7pt">
  <td width="349" valign="top" style="width:261.8pt;border-top:none;border-left:
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt;height:17.7pt">
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">AdaptiveMaxPool2d<o:p></o:p></span></p>
  </td>
  <td width="113" valign="top" style="width:3.0cm;border-top:none;border-left:none;
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt;height:17.7pt">
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">1<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style="mso-yfti-irow:12;height:17.7pt">
  <td width="349" valign="top" style="width:261.8pt;border-top:none;border-left:
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt;height:17.7pt">
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">Shared Conv:
  Conv2d 1 x 1<o:p></o:p></span></p>
  </td>
  <td width="113" valign="top" style="width:3.0cm;border-top:none;border-left:none;
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt;height:17.7pt">
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">2<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style="mso-yfti-irow:13;height:17.7pt">
  <td width="349" valign="top" style="width:261.8pt;border-top:none;border-left:
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt;height:17.7pt">
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">Linear Layer
  A:9D V:25D<o:p></o:p></span></p>
  </td>
  <td width="113" valign="top" style="width:3.0cm;border-top:none;border-left:none;
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt;height:17.7pt">
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">1<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style="mso-yfti-irow:14;height:17.45pt">
  <td width="218" rowspan="4" style="width:163.5pt;border:solid windowtext 1.0pt;
  border-top:none;mso-border-top-alt:solid windowtext .5pt;mso-border-alt:solid windowtext .5pt;
  padding:0cm 5.4pt 0cm 5.4pt;height:17.45pt">
  <p class="MsoNormal" align="center" style="text-align:center"><span class="GramE"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">MBF<span style="mso-spacerun:yes">&nbsp; </span>x</span></span><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">4<o:p></o:p></span></p>
  </td>
  <td width="349" valign="top" style="width:261.8pt;border-top:none;border-left:
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt;height:17.45pt">
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">AdaptiveAvgPool1d<o:p></o:p></span></p>
  </td>
  <td width="113" valign="top" style="width:3.0cm;border-top:none;border-left:none;
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt;height:17.45pt">
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">2<o:p></o:p></span></p>
  </td>
  <td width="246" valign="top" style="width:184.25pt;border-top:none;border-left:
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt;height:17.45pt">
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">A: 1 x <span class="GramE">TA<span style="mso-spacerun:yes">&nbsp; </span>V</span>: 1 x TV<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style="mso-yfti-irow:15;height:18.55pt">
  <td width="349" valign="top" style="width:261.8pt;border-top:none;border-left:
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt;height:18.55pt">
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">Fully Connected:
  A: 25D V: 9D<o:p></o:p></span></p>
  </td>
  <td width="113" valign="top" style="width:3.0cm;border-top:none;border-left:none;
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt;height:18.55pt">
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">2<o:p></o:p></span></p>
  </td>
  <td width="246" valign="top" style="width:184.25pt;border-top:none;border-left:
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt;height:18.55pt">
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">A: 1 x <span class="GramE">TV<span style="mso-spacerun:yes">&nbsp; </span>V</span>: 1 x TA<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style="mso-yfti-irow:16;height:17.45pt">
  <td width="349" valign="top" style="width:261.8pt;border-top:none;border-left:
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt;height:17.45pt">
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">Con2d 1x3
  stride=1 padding=1<o:p></o:p></span></p>
  </td>
  <td width="113" valign="top" style="width:3.0cm;border-top:none;border-left:none;
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt;height:17.45pt">
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">2<o:p></o:p></span></p>
  </td>
  <td width="246" valign="top" style="width:184.25pt;border-top:none;border-left:
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt;height:17.45pt">
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">A: 1 x 64<span style="mso-spacerun:yes">&nbsp;&nbsp; </span>V: 1 x 64<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style="mso-yfti-irow:17;height:18.55pt">
  <td width="349" valign="top" style="width:261.8pt;border-top:none;border-left:
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt;height:18.55pt">
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">256D Dense Layer<o:p></o:p></span></p>
  </td>
  <td width="113" valign="top" style="width:3.0cm;border-top:none;border-left:none;
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt;height:18.55pt">
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">1<o:p></o:p></span></p>
  </td>
  <td width="246" valign="top" style="width:184.25pt;border-top:none;border-left:
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt;height:18.55pt">
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">1 x 128<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style="mso-yfti-irow:18;height:6.3pt">
  <td width="218" rowspan="2" style="width:163.5pt;border:solid windowtext 1.0pt;
  border-top:none;mso-border-top-alt:solid windowtext .5pt;mso-border-alt:solid windowtext .5pt;
  padding:0cm 5.4pt 0cm 5.4pt;height:6.3pt">
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">Regression Layer
  x1<o:p></o:p></span></p>
  </td>
  <td width="349" valign="top" style="width:261.8pt;border-top:none;border-left:
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt;height:6.3pt">
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">64D Fully Connected<o:p></o:p></span></p>
  </td>
  <td width="113" valign="top" style="width:3.0cm;border-top:none;border-left:none;
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt;height:6.3pt">
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">1<o:p></o:p></span></p>
  </td>
  <td width="246" valign="top" style="width:184.25pt;border-top:none;border-left:
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt;height:6.3pt">
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">1 x 64<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style="mso-yfti-irow:19;mso-yfti-lastrow:yes;height:17.45pt">
  <td width="349" valign="top" style="width:261.8pt;border-top:none;border-left:
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt;height:17.45pt">
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">Linear
  regression<o:p></o:p></span></p>
  </td>
  <td width="113" valign="top" style="width:3.0cm;border-top:none;border-left:none;
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt;height:17.45pt">
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">1<o:p></o:p></span></p>
  </td>
  <td width="246" valign="top" style="width:184.25pt;border-top:none;border-left:
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt;
  mso-border-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt;height:17.45pt">
  <p class="MsoNormal" align="center" style="text-align:center"><span lang="EN-US" style="font-size:12.0pt;font-family:&quot;Times New Roman&quot;,serif">1<o:p></o:p></span></p>
  </td>
 </tr>
</tbody></table>

A：Audio V: Visual
