java c
EE1002 Principles of Electrical Engineering (2024/25A) 
Lab C – RC Circuit
Safety Precautions 
• Refer   to   the   departmental      and   university    safety   regulations.    Report   to   the   lab   demonstrators immediately in case of   any irregularities.
• In   the   rare   event   of   electric   shock, one   should   be   removed   from   the   source   and   the current should be shut down   immediately.
• Before   touching any circuit elements, ensure that it is not connected to high voltages. We   only   need   to   deal   with   voltages   below   20 V   in   this   course.
• When   using   the   DC   power   supply, dial   the   voltages   to   zero   before   switching   it   and   before connecting   the circuit. Double   check your circuit before dialing up   the voltage from zero.
• Electrolytic   capacitors   CANNOT   be   connected   to   a   reverse   voltage.Acknowledgment – This version is largely based on the lab reports before this semester.
I. OBJECTIVES 
1. To measure time-varying voltages using an analog oscilloscope.
2. To study the amplitude response of   an RC circuit   as   a   function of   frequency.
3. To study the phase response of   an RC circuit as   a   function   of   frequency.
II. EQUIPMENT 
1.   Signal generator SG (Model:    )
2. Real-time   Analog Oscilloscope OSC (Model:    )
3. Digital Multimeter (Model: ________________________________)
4. BNC   cable
5.   Solderless breadboard
6. Components: Resistor R=1 kΩ; Capacitor C= 0.l      μF.Check: Using the multimeter to verify the values of   R=                           and C =                           .
The correct mode is needed for measuring C.


III. BACKGROUND An AC voltage   is   a   sinusoid with   a period T. For RC   circuit,   the   characteristic   time   is   RC   according   to   Chapter   8. When   the AC   voltage   drives   the   RC   circuit, the behavior   depends   on   the   comparison   of T and RC.
•         If   T   >> RC, then   the   capacitor   behaves   as   an   open-circuit.
•         If   T   << RC, then the capacitor behaves as an short-circuit.
The   resultant   circuit   can   be   applied   as   a   low-pass   filter,   where   only   signals   at   low frequencies can pass through. Here, RC =    sec   so we   expect   interesting transition to appear when the frequency crosses (2πRC)-1   =  Hz.
IV. PROCEDURES (Items with # can be done   after the   lab)
First   write down the   names/SID of   your group members, the   venue, and the seat number.
(A) Sinusoidal Signal Measurements 
0. Look   at   OSC   carefully. It   has   10 horizontal   divisions   and   8 vertical   divisions, right?
1. To   begin   with, prepare   OSC   for   measuring   the   signals   as   follows:
(a)   Power/CRT   Panels:   Turn   on   the   cathode   ray   (i.e.   electron   beam). Adjust   beam intensity and focus   knobs.
(b) Vertical   Panel: Choose   VERT   MODE   = CH1   for   seeing   only   CH1.
(c)   CH1   Subpanel: VOLT/DIV   = 0.5 V/div.   Select “DC” to   avoid   internal   filtering.   (d) Horizontal   panel: MAIN   TIME/DIV   to 1 ms/div. Ignore   the   delay   options.
(e)   Trigger   Panel   (top):
• Source   = CH1;   Coupling   = AUTO
• Hold   Off   =   minimized   (i.e.   pushed   in   and   fully   counter-clockwise)
• MAIN   kept   at   MAIN   mode   (i.e.   not   the   MIX,   DELAY,   or   XY   modes)
• Position   ~   12-o’clock   (i.e.   default   position   for   horizontally   centering)
All of   the three small red-knobs for VAR are for   the purposes   of   fine   measurements   only. Push them in to   avoid   unwanted   magnification. Turn them clockwise fully   for locking to calibrated measurements.Follow the steps above carefully. Then, take a picture of OSC for record.   1
2.   Connect   the   SG   directly   to   CH1   of OSC.   Use   the   multimeter   to   verify   that   the   casing of SG and OSC   are both   shorted.
3. Before   enabling   the   output   of   SG,
(a)   sine   wave,
(b) frequency f = 0.2 kHz,   and
(c) peak-to-peak   amplitude   V1pp   ~2.5 V   by:
•       tuning   to   the   nine-o’clock   position   (Topward   SG)   or
•         setting   amplitude   of   ~2.5 V (Rigol   SG)
The   rest   of   SG   should   be   left   at   the   default   of:   No   attenuation   (i.e.   0   dB   without pushing) and   zero-offset   (Topward   SG) or   Offset   =0   and   Phase   =   0   (Rigol   SG)


Take a picture of SG for record.
#4. The expected signal V1(t) is shown below. Write down its mathematical formula.

Fig.   1.   Signal from   SG V1(t) expected   mathematically.

Fig. 2.   Signal from   SG V1(t) as expected experimentally.






5.   Enable   the   output   of   SG,   do   the   following   to   yield   the   expected   experimental   signal   (as   illustrated   in   Fig.   2):
(a)   Tune   CH1 position   so   that   the   sine   function   is   vertically   centered
(b)   Check   the   zero   by   momentarily   switching   from   DC   to   GND   (and   back   to   DC).
(c)   Tune   trigger   level   (top) so   that   the   trace   starting   from   zero   with   a   positive   slope.   Note   here   that triggering is   very   important   in   providing   OSC   with   a   reference   starting time for each repetition.
Carefully obtain the代 写EE1002 Principles of Electrical Engineering (2024/25A)Haskell
代做程序编程语言 exact trace in Fig. 2. Then, take a clear picture for record.
6. Experimentally, record:
Total   number   of   horizontal   divisions   for   one   full   cycle   X   = 5   div.
Total   number   of   vertical   divisions   from   the   minimum   to   maximum   Y=   div.
#7. Calculate   using   the   above:
The measured V1pp = Y × 0.5 V/div. =   Volts
The   measured   period T =X × 1 ms/div. =    seconds
These   values   in   bold   have   been   adopted   in   step   A1(c)   and   A1(d).
#8. Does   the   answer   obey   T   =   1/f?   What   is   the   relative   error?   Provide   an   explanation if   there   are   errors.
(B) Input-Output Measurements
In the following circuit,   SG provides V1(t) as   the input and the voltage V2(t) across the   capacitor   is   regarded   as   the   output.





Fig.   3.   The   input V1(t)    from    SG    and    output V2(t)   across the capacitor.

Fig. 4. Expected input V1(t) and V2(t).   Period   of T and   time   shift   of ∆t.


Both   V1    and   V2 are   expected   to   have   the   same   period   T.   However,   the   output   V2      is   expected   to   have   a   smaller   amplitude   and   a   time   shift   of   ∆t.
1. Build the   above RC circuit, including the   connection   to   SG   and   OSC   via   two   BNC   cables.   Check   that   the   shielding   of the   BNC   cables   (i.e.   usually   linked   to   the   black alligator   clip) are   correctly   connected   to   the   node   at   the   bottom   in   Fig.   3.
2. On OSC, switch   to   showing   CH2   as   follows:
(a)   Vertical   Panel: Choose   VERT   MODE   = CH2 for   seeing   only   CH2.
(b)   CH2   Subpanel: VOLT/DIV   =0.5 V/div.   Select “DC” that   stands   for   no   internal filtering.
(c)   Tune   CH2 position   so   that   the   sine   function   is   vertically   centered.
(d)   Check   the   zero   by   momentarily   switching   from   DC   to   GND   (and   back   to   DC).         Other   Panels: No   change. The   trigger   should   NOT   be   changed. It   should   continue   to   be   based   on   CH1.
The trace should look like Fig. 5(a). Take a clear picture for record.

Fig. 5. (a) CH2 only and   (b)   CH1      CH2 that   are   very   close to   each   other.


3. On OSC, switch to showing both CH1 and CH2 by setting VERT MODE = DUAL.
The traces are very close to each other (Fig. 5(b)). Take a picture for record.
4.   Keep   VOLT/DIV   for   both   CH1   and   CH2   as   0.5 V/div.   Fill   out   Table   I.   Only   the boxes in gray have to be completed   during the   lab   session.
Table I Basic Data points at 200 Hz, 2 kHz, 20 kHz,   and   200 kHz

Take pictures for the time trace for each case.       Examples are shown below Fig.6.

Fig. 6. CH1    CH2   at   different   frequencies.




5. As   an   option, more   data   points   can   be   taken   for   Tables   II   and   III.
Table II   Additional data points at 400 Hz, 4 kHz, 40 kHz,   and 400   kHz




Table III Additional data points at 700 Hz, 7 kHz, 70 kHz, and 700 kHz



#6. From   the   experimental   data,
(a)   plot   the   V2pp/V1pp   versus   f
(b) plot   the   ϕ versus   f
Mark   on   both   plots   fc   =   1/(2πRC) as   the   characteristic   frequency   determined   by   the RC time.




V. DISCUSSIONS 
1.       As   bonus,   set   SG   to   500   Hz   with   a   square   wave.   Then   determine   the   RC   time   constant from OSC. Example of   the time trace is   shown in   Fig.   7   .

Fig. 7. CH2 obtained from   a   square-wave input   at   500   Hz.
2. Comment on   the   physical   reason for   the low-frequency and   high-frequency   behaviors   of   CH2. Then, suggest   one   application   of   the   RC   circuit.
VI. REFERENCES 
•          "Modern   Instrumentation   and      Measurement   Techniques"   by   Helfrick,   A.D.   and Cooper, W.D.: Chapter 7,   Sections   1, 2, 4,   and   10.1.
•         "Electronic Instrumentation and Measurements" by Bell, D.   A. Chapter 11, Sections   1-4   and   6.


VII. Instructions for Preparing the Formal Report: 
The    following    serves    as      a      rough      guideline      for      formal      report.      More      professional   guidelines would be necessary in the future.
1.       Format:   At least 9 pages, single-spaced,   12-points Times New Romans (PDF).
2.       DO   NOT   JUST   HAND   IN   THIS   DOCUMENT!!! No   part   of   the   formal   report can contain sentences   in this   document.
3.       The procedural steps should be expressed in passive voice   and in past   tense.   (e.g. The time scale of   the oscilloscope was set to   1   ms/div.)
4.       Figures: Must include labeled axes, units, legends, and   caption.
5.       Tables: Must include units, legends, and   caption
6.         Content:
•         Title   of   the   report
•         Name   of   all   group   members
•         Date, time, and   venue
•         Objective,       Background,          Procedure       and          Results,       Discussions.       They   correspond to   Sections I-V of   this document.
•         Add   a   conclusion   (and   a   reference   list   if   necessary)
7.       Checking: The items marked by (*) have to be included.

         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
