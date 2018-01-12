This is the ipython script for Daily sports and Activity dataset. 

UCI Machine Learning Repository: Daily and Sports Activities Data Set
Billur Barshan,
Department of Electrical and Electronics Engineering, Bilkent University, TR-06800 Bilkent, Ankara, Turkey
tel: (90-312) 290-2161 fax: (90-312) 266-4192 e-mail : billur`@'ee.bilkent.edu.tr
url: www.ee.bilkent.edu.tr/~billur
Kerem Altun, kerem.altun '@' kemerburgaz.edu.tr, kerem.altun '@' gmail.com
Brief Description of the Dataset:
---------------------------------
Each of the 19 activities is performed by eight subjects (4 female, 4 male, between the ages 20 and 30) for 5 minutes.
Total signal duration is 5 minutes for each activity of each subject.
The subjects are asked to perform the activities in their own style and were not restricted on how the activities should be performed. For this reason, there are inter-subject variations in the speeds and amplitudes of some activities.
The activities are performed at the Bilkent University Sports Hall, in the Electrical and Electronics Engineering Building,
and in a flat outdoor area on campus. Sensor units are calibrated to acquire data at 25 Hz sampling frequency. The 5-min signals are divided into 5-sec segments so that 480(=60x8) signal segments are obtained for each activity.
The 19 activities are: sitting (A1),

UCI Machine Learning Repository: Daily and Sports Activities Data Set
22/04/17, 15*47
standing (A2),
lying on back and on right side (A3 and A4),
ascending and descending stairs (A5 and A6),
standing in an elevator still (A7)
and moving around in an elevator (A8),
walking in a parking lot (A9),
walking on a treadmill with a speed of 4 km/h (in flat and 15 deg inclined positions) (A1
0 and A11),
running on a treadmill with a speed of 8 km/h (A12),
exercising on a stepper (A13),
exercising on a cross trainer (A14),
cycling on an exercise bike in horizontal and vertical positions (A15 and A16),
rowing (A17),
jumping (A18),
and playing basketball (A19).
File structure:
19 activities (a) (in the order given above)
8 subjects (p)
60 segments (s)
5 units on torso (T), right arm (RA), left arm (LA), right leg (RL), left leg (LL)
9 sensors on each unit (x,y,z accelerometers, x,y,z gyroscopes, x,y,z magnetometers)
Folders a01, a02, ..., a19 contain data recorded from the 19 activities.
For each activity, the subfolders p1, p2, ..., p8 contain data from each of the 8 subjects.


UCI Machine Learning Repository: Daily and Sports Activities Data Set 22/04/17, 15*47
In each subfolder, there are 60 text files s01, s02, ..., s60, one for each segment.
In each text file, there are 5 units x 9 sensors = 45 columns and 5 sec x 25 Hz = 125 rows.
Each column contains the 125 samples of data acquired from one of the sensors of one of the units over a period of 5 sec.
Each row contains data acquired from all of the 45 sensor axes at a particular sampling instant separated by commas.
Columns 1-45 correspond to:
T_xacc, T_yacc, T_zacc, T_xgyro, ..., T_ymag, T_zmag,
RA_xacc, RA_yacc, RA_zacc, RA_xgyro, ..., RA_ymag, RA_zmag, LA_xacc, LA_yacc, LA_zacc, LA_xgyro, ..., LA_ymag, LA_zmag, RL_xacc, RL_yacc, RL_zacc, RL_xgyro, ..., RL_ymag, RL_zmag, LL_xacc, LL_yacc, LL_zacc, LL_xgyro, ..., LL_ymag, LL_zmag.

Therefore,
columns 1-9 correspond to the sensors in unit 1 (T),
columns 10-18 correspond to the sensors in unit 2 (RA), 
columns 19-27 correspond to the sensors in unit 3 (LA), 
columns 28-36 correspond to the sensors in unit 4 (RL), 
columns 37-45 correspond to the sensors in unit 5 (LL).