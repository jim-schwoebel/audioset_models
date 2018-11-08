# audioset-models
List of models built with machine learning scripts from the [voicebook](https://github.com/jim-schwoebel/voicebook) repository, trained on [download_audioset](https://github.com/jim-schwoebel/download_audioset) folders. 

## how dataset was made
The dataset was made making a variable dataset and a control dataset composed of an equal mixture of all the other classes. In this way, it was assumed that all classes are equally probable in the wild. 

The goal here was just to see which groups are most easily separated from the rest and generally to see which algorithms work best on a MFCC-based feature embedding, as described by train_audioclassify.py script in the [Chapter 4: Modeling](https://github.com/jim-schwoebel/voicebook/tree/master/chapter_4_modeling) chapter of the [Voicebook](ttps://github.com/jim-schwoebel/voicebook).

## performance of models 

Here are the performance of the models, from least accurate to most accurate. 

| Model Name | Accuracy | Standard Deviation | Modeltype |
|-----|-----|-----|-----|
| Fly,housefly_Fly,housefly_controls_sc_audio | 0.5391666666666668 | 0.0607590871118606 | knn |
| Neigh,whinny_Neigh,whinny_controls_sc_audio | 0.5424603174603174 | 0.06308899839367364 | knn |
| Squeal_Squeal_controls_sc_audio | 0.5507936507936508 | 0.026370234485454197 | sk |
| Shout_Shout_controls_sc_audio | 0.5511904761904762 | 0.1665645945942162 | logistic regression |
| Fire_Fire_controls_sc_audio | 0.555952380952381 | 0.17194220524663026 | gaussian-nb |
| Crackle_Crackle_controls_sc_audio | 0.5650793650793651 | 0.007776157913597362 | sk |
| Bleat_Bleat_controls_sc_audio | 0.5682539682539682 | 0.006349206349206327 | sk |
| Outside,ruralornatural_Outside,ruralornatural_controls_sc_audio | 0.5797794117647059 | 0.08903285375883954 | logistic regression |
| Whitenoise_Whitenoise_controls_sc_audio | 0.5932539682539683 | 0.07245731838922985 | decision-tree |
| Bell_Bell_controls_sc_audio | 0.5944444444444444 | 0.10859973640061793 | logistic regression |
| Buzz_Buzz_controls_sc_audio | 0.5968253968253967 | 0.10793650793650796 | adaboost |
| Pulse_Pulse_controls_sc_audio | 0.5988095238095237 | 0.14704188244423344 | hard voting |
| Slosh_Slosh_controls_sc_audio | 0.6 | 0.1457737973711325 | gaussian-nb |
| Rattle_Rattle_controls_sc_audio | 0.6051587301587302 | 0.15738517472263444 | gaussian-nb |
| Glass_Glass_controls_sc_audio | 0.6063492063492063 | 0.1881245372666572 | decision-tree |
| Moo_Moo_controls_sc_audio | 0.6079365079365079 | 0.12694443824210921 | hard voting |
| Scrape_Scrape_controls_sc_audio | 0.6087301587301588 | 0.2253968253968254 | gradient boosting |
| Snake_Snake_controls_sc_audio | 0.6095238095238095 | 0.12360585608845578 | random forest |
| Alarm_Alarm_controls_sc_audio | 0.611111111111111 | 0.19465084607328867 | logistic regression |
| Clip-clop_Clip-clop_controls_sc_audio | 0.6115079365079366 | 0.16315460627269146 | random forest |
| Animal_Animal_controls_sc_audio | 0.6165522763669641 | 0.04032022431311725 | knn |
| Clapping_Clapping_controls_sc_audio | 0.619047619047619 | 0.1412609235637269 | adaboost |
| Horse_Horse_controls_sc_audio | 0.6202020202020202 | 0.19362348007281188 | gaussian-nb |
| Microwaveoven_Microwaveoven_controls_sc_audio | 0.6202380952380953 | 0.09991492980170137 | decision-tree |
| Sheep_Sheep_controls_sc_audio | 0.6214285714285714 | 0.13044273119821195 | gradient boosting |
| Hum_Hum_controls_sc_audio | 0.6219780219780219 | 0.09953399449867475 | knn |
| Pig_Pig_controls_sc_audio | 0.6226190476190475 | 0.08464947064110084 | random forest |
| Creak_Creak_controls_sc_audio | 0.6238095238095238 | 0.1493751156319821 | random forest |
| Bow-wow_Bow-wow_controls_sc_audio | 0.6246031746031745 | 0.13368599430877576 | knn |
| Livestock,farmanimals,workinganimals_Livestock,farmanimals,workinganimals_controls_sc_audio | 0.6246568627450981 | 0.03805247898951148 | hard voting |
| Inside,largeroomorhall_Inside,largeroomorhall_controls_sc_audio | 0.6256709956709956 | 0.10152725169949675 | gaussian-nb |
| Echo_Echo_controls_sc_audio | 0.6285714285714284 | 0.2138089935299395 | logistic regression |
| Femalesinging_Femalesinging_controls_sc_audio | 0.6285714285714287 | 0.11070219539150918 | knn |
| Door_Door_controls_sc_audio | 0.6333333333333333 | 0.08079466429027214 | adaboost |
| Growling_Growling_controls_sc_audio | 0.6333333333333333 | 0.08079466429027216 | knn |
| Tubularbells_Tubularbells_controls_sc_audio | 0.6333333333333333 | 0.1379412113103904 | knn |
| Mainshum_Mainshum_controls_sc_audio | 0.6333333333333334 | 0.11967032904743341 | knn |
| Burst,pop_Burst,pop_controls_sc_audio | 0.6341269841269841 | 0.2517656220484684 | random forest |
| Insect_Insect_controls_sc_audio | 0.6346320346320347 | 0.14793716884164887 | gaussian-nb |
| Radio_Radio_controls_sc_audio | 0.6349206349206349 | 0.23414716082013684 | decision-tree |
| Music_Music_controls_sc_audio | 0.6349478387347549 | 0.026775070319852455 | logistic regression |
| Malletpercussion_Malletpercussion_controls_sc_audio | 0.6369047619047619 | 0.06692128248835807 | hard voting |
| MusicofLatinAmerica_MusicofLatinAmerica_controls_sc_audio | 0.6369047619047619 | 0.15856141824545172 | knn |
| Breathing_Breathing_controls_sc_audio | 0.6380952380952382 | 0.05714285714285716 | hard voting |
| Wildanimals_Wildanimals_controls_sc_audio | 0.6380952380952382 | 0.20213025244103625 | knn |
| Rattle(instrument)_Rattle(instrument)_controls_sc_audio | 0.6404761904761905 | 0.047708249784556865 | knn |
| Chink,clink_Chink,clink_controls_sc_audio | 0.6412698412698413 | 0.08786255557522572 | adaboost |
| Smash,crash_Smash,crash_controls_sc_audio | 0.6412698412698413 | 0.08786255557522572 | gradient boosting |
| Coo_Coo_controls_sc_audio | 0.6428571428571429 | 0.1577549406997852 | gaussian-nb |
| Tambourine_Tambourine_controls_sc_audio | 0.6428571428571429 | 0.1784567533022882 | logistic regression |
| Slidingdoor_Slidingdoor_controls_sc_audio | 0.6444444444444445 | 0.06853026395213621 | knn |
| Toot_Toot_controls_sc_audio | 0.6460317460317461 | 0.09933008156928265 | adaboost |
| Outside,urbanormanmade_Outside,urbanormanmade_controls_sc_audio | 0.646401515151515 | 0.07026387526407724 | gaussian-nb |
| Ping_Ping_controls_sc_audio | 0.6476190476190476 | 0.06459361888690734 | gradient boosting |
| Basketballbounce_Basketballbounce_controls_sc_audio | 0.65 | 0.2 | hard voting |
| Musicalinstrument_Musicalinstrument_controls_sc_audio | 0.6501863354037267 | 0.04685526636548159 | gaussian-nb |
| Cowbell_Cowbell_controls_sc_audio | 0.6515873015873016 | 0.07679981208509806 | gradient boosting |
| Inside,publicspace_Inside,publicspace_controls_sc_audio | 0.653968253968254 | 0.21517159622641957 | knn |
| Pour_Pour_controls_sc_audio | 0.6555555555555554 | 0.15660582437369686 | gaussian-nb |
| Skidding_Skidding_controls_sc_audio | 0.655952380952381 | 0.1568720610478965 | random forest |
| Clock_Clock_controls_sc_audio | 0.6563492063492063 | 0.11871249125829522 | gaussian-nb |
| Fart_Fart_controls_sc_audio | 0.6563492063492063 | 0.1688369654041237 | knn |
| Electricpiano_Electricpiano_controls_sc_audio | 0.657936507936508 | 0.10998293461155562 | logistic regression |
| Blender_Blender_controls_sc_audio | 0.6583333333333333 | 0.0927960727138337 | hard voting |
| Spray_Spray_controls_sc_audio | 0.6583333333333333 | 0.1452966314513558 | knn |
| Traditionalmusic_Traditionalmusic_controls_sc_audio | 0.6583333333333333 | 0.16541194367732673 | knn |
| Boat,Watervehicle_Boat,Watervehicle_controls_sc_audio | 0.6585105083088953 | 0.06257911638839117 | logistic regression |
| Percussion_Percussion_controls_sc_audio | 0.6588235294117648 | 0.06056253024110002 | hard voting |
| Printer_Printer_controls_sc_audio | 0.6591269841269841 | 0.12625285470331238 | gaussian-nb |
| Vehiclehorn,carhorn,honking_Vehiclehorn,carhorn,honking_controls_sc_audio | 0.6591269841269841 | 0.16864098944425018 | logistic regression |
| Tap_Tap_controls_sc_audio | 0.6595238095238096 | 0.19289388244996605 | decision-tree |
| Snort_Snort_controls_sc_audio | 0.6603174603174603 | 0.1280117152613076 | logistic regression |
| Television_Television_controls_sc_audio | 0.6619047619047619 | 0.19886298112210574 | logistic regression |
| Churchbell_Churchbell_controls_sc_audio | 0.6623015873015874 | 0.22807071479000185 | gaussian-nb |
| Pluckedstringinstrument_Pluckedstringinstrument_controls_sc_audio | 0.6632456140350877 | 0.042849913328679094 | adaboost |
| Icecreamtruck,icecreamvan_Icecreamtruck,icecreamvan_controls_sc_audio | 0.6642857142857143 | 0.17401325307256904 | random forest |
| Electrictoothbrush_Electrictoothbrush_controls_sc_audio | 0.6654761904761906 | 0.0632634774075544 | logistic regression |
| Water_Water_controls_sc_audio | 0.6664332399626517 | 0.08412577164657657 | knn |
| Gush_Gush_controls_sc_audio | 0.6666666666666666 | 0.1257880174994219 | hard voting |
| Birdvocalization,birdcall,birdsong_Birdvocalization,birdcall,birdsong_controls_sc_audio | 0.6666666666666667 | 0.07388575599039104 | adaboost |
| Keysjangling_Keysjangling_controls_sc_audio | 0.6666666666666667 | 0.0875177698545411 | adaboost |
| Inside,smallroom_Inside,smallroom_controls_sc_audio | 0.6680029861888764 | 0.021672207908822894 | random forest |
| Roaringcats(lions,tigers)_Roaringcats(lions,tigers)_controls_sc_audio | 0.6698412698412698 | 0.12311567891850994 | gaussian-nb |
| Airhorn,truckhorn_Airhorn,truckhorn_controls_sc_audio | 0.6730158730158731 | 0.1093280975093496 | gaussian-nb |
| Sawing_Sawing_controls_sc_audio | 0.6738095238095237 | 0.06004533434723093 | random forest |
| Motorcycle_Motorcycle_controls_sc_audio | 0.6746031746031745 | 0.16403823089223887 | random forest |
| Mouse_Mouse_controls_sc_audio | 0.6749999999999999 | 0.22257766358404119 | knn |
| Bellow_Bellow_controls_sc_audio | 0.675 | 0.1 | adaboost |
| Housemusic_Housemusic_controls_sc_audio | 0.675 | 0.12747548783981963 | knn |
| Roar_Roar_controls_sc_audio | 0.675 | 0.1695582495781317 | knn |
| Whip_Whip_controls_sc_audio | 0.6753968253968254 | 0.13056460141383358 | gaussian-nb |
| Machinegun_Machinegun_controls_sc_audio | 0.6761904761904762 | 0.26289315660812324 | gaussian-nb |
| Draweropenorclose_Draweropenorclose_controls_sc_audio | 0.6773809523809524 | 0.03375582590180436 | gaussian-nb |
| Squish_Squish_controls_sc_audio | 0.6801587301587302 | 0.1128994406481478 | hard voting |
| Tick-tock_Tick-tock_controls_sc_audio | 0.6801587301587302 | 0.1202479172477376 | hard voting |
| Speech_Speech_controls_sc_audio | 0.6802220708103061 | 0.010800269230362968 | logistic regression |
| Sizzle_Sizzle_controls_sc_audio | 0.6805555555555555 | 0.19492974747325614 | random forest |
| Drum_Drum_controls_sc_audio | 0.6806666666666666 | 0.057836935526626165 | logistic regression |
| Childspeech,kidspeaking_Childspeech,kidspeaking_controls_sc_audio | 0.6811145510835913 | 0.09009234730088819 | gaussian-nb |
| Bird_Bird_controls_sc_audio | 0.6822134387351778 | 0.05418624921474027 | logistic regression |
| Jinglebell_Jinglebell_controls_sc_audio | 0.6825396825396824 | 0.11707358041006842 | knn |
| Cacophony_Cacophony_controls_sc_audio | 0.6825396825396826 | 0.1104287436884196 | gradient boosting |
| Mosquito_Mosquito_controls_sc_audio | 0.6833333333333333 | 0.12527746981977425 | adaboost |
| Run_Run_controls_sc_audio | 0.6833333333333333 | 0.1527525231651947 | logistic regression |
| Chirptone_Chirptone_controls_sc_audio | 0.6849206349206349 | 0.16979954241897746 | gradient boosting |
| Emergencyvehicle_Emergencyvehicle_controls_sc_audio | 0.6860681114551084 | 0.11124162561136779 | gradient boosting |
| Wood_Wood_controls_sc_audio | 0.6862789384528515 | 0.08689517865166056 | hard voting |
| Hiss_Hiss_controls_sc_audio | 0.6873626373626374 | 0.0941071195768474 | gaussian-nb |
| Mandolin_Mandolin_controls_sc_audio | 0.6876984126984127 | 0.07765620560252419 | gaussian-nb |
| Duck_Duck_controls_sc_audio | 0.6888888888888889 | 0.11340045142534445 | knn |
| Meow_Meow_controls_sc_audio | 0.6888888888888889 | 0.11340045142534445 | random forest |
| Country_Country_controls_sc_audio | 0.6896825396825397 | 0.1500902558730489 | random forest |
| Mechanisms_Mechanisms_controls_sc_audio | 0.6897619047619048 | 0.12001417149880347 | decision-tree |
| Saxophone_Saxophone_controls_sc_audio | 0.6904761904761905 | 0.1035782701626486 | gaussian-nb |
| Goose_Goose_controls_sc_audio | 0.6911111111111111 | 0.10650740425197595 | knn |
| Crying,sobbing_Crying,sobbing_controls_sc_audio | 0.6916666666666667 | 0.11666666666666668 | gaussian-nb |
| Drip_Drip_controls_sc_audio | 0.6916666666666667 | 0.2 | logistic regression |
| Helicopter_Helicopter_controls_sc_audio | 0.692063492063492 | 0.1734739821246254 | hard voting |
| Marimba,xylophone_Marimba,xylophone_controls_sc_audio | 0.6927272727272727 | 0.11360363164955135 | logistic regression |
| Bee,wasp,etc._Bee,wasp,etc._controls_sc_audio | 0.6928571428571428 | 0.1660153562580265 | knn |
| Ringtone_Ringtone_controls_sc_audio | 0.6932539682539682 | 0.10855622747014451 | hard voting |
| Typewriter_Typewriter_controls_sc_audio | 0.6932539682539682 | 0.1187403441858098 | knn |
| Telephonedialing,DTMF_Telephonedialing,DTMF_controls_sc_audio | 0.694047619047619 | 0.043513492577373976 | knn |
| Single-lensreflexcamera_Single-lensreflexcamera_controls_sc_audio | 0.6952380952380952 | 0.09331389496316869 | adaboost |
| Slap,smack_Slap,smack_controls_sc_audio | 0.6952380952380953 | 0.10795984808337748 | adaboost |
| Windinstrument,woodwindinstrument_Windinstrument,woodwindinstrument_controls_sc_audio | 0.6956439393939393 | 0.06460415775525118 | gaussian-nb |
| Gasp_Gasp_controls_sc_audio | 0.6984126984126984 | 0.1447841809649699 | gaussian-nb |
| Pinknoise_Pinknoise_controls_sc_audio | 0.6984126984126984 | 0.170662603882103 | gaussian-nb |
| Acapella_Acapella_controls_sc_audio | 0.6996031746031747 | 0.051367051191379076 | adaboost |
| Burping,eructation_Burping,eructation_controls_sc_audio | 0.7 | 0.1274754878398196 | decision-tree |
| Femalespeech,womanspeaking_Femalespeech,womanspeaking_controls_sc_audio | 0.7 | 0.1695582495781317 | gaussian-nb |
| Gurgling_Gurgling_controls_sc_audio | 0.7 | 0.1695582495781317 | gaussian-nb |
| Pulleys_Pulleys_controls_sc_audio | 0.7 | 0.2318404623873926 | logistic regression |
| Car_Car_controls_sc_audio | 0.7000693000693001 | 0.05437896557292015 | hard voting |
| Dog_Dog_controls_sc_audio | 0.7005415499533146 | 0.07139205965268808 | gradient boosting |
| Ding-dong_Ding-dong_controls_sc_audio | 0.7011904761904761 | 0.04885305840162665 | knn |
| Chicken,rooster_Chicken,rooster_controls_sc_audio | 0.703030303030303 | 0.06470956516382616 | knn |
| Cluck_Cluck_controls_sc_audio | 0.7047619047619047 | 0.09233675918888246 | gaussian-nb |
| Firecracker_Firecracker_controls_sc_audio | 0.7047619047619047 | 0.09233675918888246 | knn |
| Goat_Goat_controls_sc_audio | 0.7047619047619047 | 0.17692539419800346 | random forest |
| Cutlery,silverware_Cutlery,silverware_controls_sc_audio | 0.7055555555555555 | 0.19421593310593657 | gradient boosting |
| Stomachrumble_Stomachrumble_controls_sc_audio | 0.7059523809523809 | 0.12329333787976089 | decision-tree |
| Zing_Zing_controls_sc_audio | 0.7059523809523809 | 0.14646244284980667 | random forest |
| Camera_Camera_controls_sc_audio | 0.705952380952381 | 0.12360585608845578 | logistic regression |
| Cattle,bovinae_Cattle,bovinae_controls_sc_audio | 0.7067460317460318 | 0.055248585028435285 | random forest |
| Vehicle_Vehicle_controls_sc_audio | 0.7073054706082229 | 0.03255966435828056 | logistic regression |
| Tabla_Tabla_controls_sc_audio | 0.7075396825396825 | 0.12816661727542253 | gaussian-nb |
| Trumpet_Trumpet_controls_sc_audio | 0.7075396825396825 | 0.23222119150461837 | random forest |
| Whoosh,swoosh,swish_Whoosh,swoosh,swish_controls_sc_audio | 0.707936507936508 | 0.1769253941980035 | knn |
| Bang_Bang_controls_sc_audio | 0.7083333333333333 | 0.052704627669472995 | gaussian-nb |
| Hoot_Hoot_controls_sc_audio | 0.7083333333333333 | 0.0950146187582615 | knn |
| Telephone_Telephone_controls_sc_audio | 0.7083333333333333 | 0.12360330811826105 | knn |
| Rub_Rub_controls_sc_audio | 0.7088888888888888 | 0.07316478948068593 | hard voting |
| Singing_Singing_controls_sc_audio | 0.7100099206349206 | 0.08037145557519358 | gaussian-nb |
| Song_Song_controls_sc_audio | 0.7103030303030302 | 0.08983291181805042 | logistic regression |
| Powerwindows,electricwindows_Powerwindows,electricwindows_controls_sc_audio | 0.711111111111111 | 0.10306465448093922 | logistic regression |
| Tiresqueal_Tiresqueal_controls_sc_audio | 0.7123015873015873 | 0.18244476483216407 | gradient boosting |
| Artilleryfire_Artilleryfire_controls_sc_audio | 0.7126984126984126 | 0.07345451404550216 | hard voting |
| Reverberation_Reverberation_controls_sc_audio | 0.7126984126984126 | 0.107914621964129 | hard voting |
| Cat_Cat_controls_sc_audio | 0.7133333333333333 | 0.055239378063921846 | hard voting |
| Owl_Owl_controls_sc_audio | 0.7134920634920635 | 0.12464108209143225 | knn |
| Tools_Tools_controls_sc_audio | 0.7138461538461538 | 0.06498065255982424 | gradient boosting |
| Crow_Crow_controls_sc_audio | 0.7166666666666667 | 0.11303883305208781 | gradient boosting |
| Zipper(clothing)_Zipper(clothing)_controls_sc_audio | 0.7166666666666667 | 0.11303883305208781 | hard voting |
| Chop_Chop_controls_sc_audio | 0.7174603174603174 | 0.1388866212966816 | logistic regression |
| Christmasmusic_Christmasmusic_controls_sc_audio | 0.7174603174603175 | 0.1054809379418168 | random forest |
| Chatter_Chatter_controls_sc_audio | 0.7178571428571429 | 0.16536909861128893 | hard voting |
| Jingle(music)_Jingle(music)_controls_sc_audio | 0.7178571428571429 | 0.16536909861128893 | knn |
| Frog_Frog_controls_sc_audio | 0.7182539682539681 | 0.10426771365025392 | gaussian-nb |
| Steelguitar,slideguitar_Steelguitar,slideguitar_controls_sc_audio | 0.7182539682539681 | 0.16491903080632095 | gaussian-nb |
| Carnaticmusic_Carnaticmusic_controls_sc_audio | 0.719047619047619 | 0.0954164995691137 | gaussian-nb |
| Timpani_Timpani_controls_sc_audio | 0.719047619047619 | 0.15565270694769856 | logistic regression |
| Sanding_Sanding_controls_sc_audio | 0.7198412698412698 | 0.08969834107178618 | decision-tree |
| Splash,splatter_Splash,splatter_controls_sc_audio | 0.7206349206349205 | 0.2593866440103555 | gaussian-nb |
| Toiletflush_Toiletflush_controls_sc_audio | 0.7214285714285714 | 0.14223076965528483 | logistic regression |
| Electricshaver,electricrazor_Electricshaver,electricrazor_controls_sc_audio | 0.7218253968253967 | 0.1362585392508318 | logistic regression |
| Lawnmower_Lawnmower_controls_sc_audio | 0.7218253968253967 | 0.2074998444267798 | random forest |
| Boiling_Boiling_controls_sc_audio | 0.7218253968253968 | 0.056125197486467125 | logistic regression |
| Quack_Quack_controls_sc_audio | 0.7222222222222222 | 0.13522957160708982 | gaussian-nb |
| Airconditioning_Airconditioning_controls_sc_audio | 0.7226190476190476 | 0.07946818699180301 | gaussian-nb |
| Vibration_Vibration_controls_sc_audio | 0.7226190476190476 | 0.07946818699180301 | logistic regression |
| Yodeling_Yodeling_controls_sc_audio | 0.7226190476190476 | 0.13716848305556262 | random forest |
| Watertap,faucet_Watertap,faucet_controls_sc_audio | 0.7236363636363636 | 0.1265404619937016 | adaboost |
| Childrenplaying_Childrenplaying_controls_sc_audio | 0.7238095238095238 | 0.06998542122237651 | adaboost |
| Harmonica_Harmonica_controls_sc_audio | 0.7238095238095238 | 0.06998542122237651 | gaussian-nb |
| Reversingbeeps_Reversingbeeps_controls_sc_audio | 0.7238095238095238 | 0.16174906924262855 | hard voting |
| Steelpan_Steelpan_controls_sc_audio | 0.7238095238095238 | 0.20612930896187845 | logistic regression |
| Thump,thud_Thump,thud_controls_sc_audio | 0.7238095238095239 | 0.09917777366230669 | adaboost |
| Fireworks_Fireworks_controls_sc_audio | 0.725 | 0.1224744871391589 | adaboost |
| Screaming_Screaming_controls_sc_audio | 0.725 | 0.1224744871391589 | knn |
| Explosion_Explosion_controls_sc_audio | 0.7253968253968254 | 0.1403303879701609 | gradient boosting |
| Giggle_Giggle_controls_sc_audio | 0.726984126984127 | 0.16840364710952183 | hard voting |
| Rockmusic_Rockmusic_controls_sc_audio | 0.7272222222222222 | 0.12237868772738389 | knn |
| Enginestarting_Enginestarting_controls_sc_audio | 0.7281746031746033 | 0.08211505548996743 | gaussian-nb |
| Pigeon,dove_Pigeon,dove_controls_sc_audio | 0.7281746031746033 | 0.12891635097223691 | logistic regression |
| Harmonic_Harmonic_controls_sc_audio | 0.7289682539682539 | 0.18841309958369185 | logistic regression |
| Shufflingcards_Shufflingcards_controls_sc_audio | 0.7309523809523809 | 0.11684874033516081 | gaussian-nb |
| Whack,thwack_Whack,thwack_controls_sc_audio | 0.7317460317460318 | 0.038276684291388884 | random forest |
| Babycry,infantcry_Babycry,infantcry_controls_sc_audio | 0.7333333333333333 | 0.08579691784155835 | random forest |
| Rainonsurface_Rainonsurface_controls_sc_audio | 0.7333333333333334 | 0.10306465448093921 | knn |
| Rowboat,canoe,kayak_Rowboat,canoe,kayak_controls_sc_audio | 0.7345238095238096 | 0.12326140371484738 | gaussian-nb |
| Slam_Slam_controls_sc_audio | 0.7345238095238096 | 0.1304970438670926 | gradient boosting |
| Soundeffect_Soundeffect_controls_sc_audio | 0.7353174603174604 | 0.2210841036845264 | knn |
| MusicofBollywood_MusicofBollywood_controls_sc_audio | 0.7357142857142858 | 0.1309307341415954 | gaussian-nb |
| Brassinstrument_Brassinstrument_controls_sc_audio | 0.7362328513162775 | 0.06545830055218035 | logistic regression |
| Gunshot,gunfire_Gunshot,gunfire_controls_sc_audio | 0.7364577451533973 | 0.09819117564665901 | hard voting |
| Snaredrum_Snaredrum_controls_sc_audio | 0.7371794871794871 | 0.1440240684100884 | gaussian-nb |
| Ship_Ship_controls_sc_audio | 0.7384920634920634 | 0.12459559172154697 | hard voting |
| Piano_Piano_controls_sc_audio | 0.7387878787878788 | 0.08806458936954427 | adaboost |
| Ambulance(siren)_Ambulance(siren)_controls_sc_audio | 0.7394444444444443 | 0.09597453365925314 | logistic regression |
| Snicker_Snicker_controls_sc_audio | 0.7396825396825397 | 0.11205944504585895 | random forest |
| Caralarm_Caralarm_controls_sc_audio | 0.7400793650793651 | 0.22507382400773385 | hard voting |
| Classicalmusic_Classicalmusic_controls_sc_audio | 0.7404761904761905 | 0.10273410238275812 | adaboost |
| Independentmusic_Independentmusic_controls_sc_audio | 0.7412698412698413 | 0.02425509014275575 | adaboost |
| Liquid_Liquid_controls_sc_audio | 0.7412698412698413 | 0.02425509014275575 | gradient boosting |
| Mechanicalfan_Mechanicalfan_controls_sc_audio | 0.7412698412698413 | 0.1437012101302384 | logistic regression |
| Boing_Boing_controls_sc_audio | 0.7416666666666667 | 0.06666666666666668 | gaussian-nb |
| Caw_Caw_controls_sc_audio | 0.7416666666666667 | 0.10341394704992381 | hard voting |
| Oink_Oink_controls_sc_audio | 0.7416666666666667 | 0.1301708279317776 | knn |
| Rustle_Rustle_controls_sc_audio | 0.7416666666666667 | 0.1522972240208089 | logistic regression |
| Squeak_Squeak_controls_sc_audio | 0.7416666666666667 | 0.21953233120532484 | logistic regression |
| Domesticanimals,pets_Domesticanimals,pets_controls_sc_audio | 0.7420604203623071 | 0.056216548281971236 | hard voting |
| Drummachine_Drummachine_controls_sc_audio | 0.7432539682539682 | 0.1623185654953233 | decision-tree |
| Drumroll_Drumroll_controls_sc_audio | 0.7433333333333334 | 0.16384274303259344 | gaussian-nb |
| Pump(liquid)_Pump(liquid)_controls_sc_audio | 0.7448412698412699 | 0.07618220854613623 | hard voting |
| Guitar_Guitar_controls_sc_audio | 0.7448880105401845 | 0.03819311865695462 | hard voting |
| Bus_Bus_controls_sc_audio | 0.746031746031746 | 0.06582997255024671 | adaboost |
| Dentaldrill,dentist'sdrill_Dentaldrill,dentist'sdrill_controls_sc_audio | 0.746031746031746 | 0.1192062435271021 | logistic regression |
| Gears_Gears_controls_sc_audio | 0.746031746031746 | 0.14373627203392728 | logistic regression |
| Hammer_Hammer_controls_sc_audio | 0.746031746031746 | 0.17474741516854456 | logistic regression |
| Scissors_Scissors_controls_sc_audio | 0.746031746031746 | 0.19231912674109156 | random forest |
| Didgeridoo_Didgeridoo_controls_sc_audio | 0.7468253968253968 | 0.02843884582090304 | knn |
| Chirp,tweet_Chirp,tweet_controls_sc_audio | 0.7476190476190476 | 0.14234033502509644 | knn |
| Noise_Noise_controls_sc_audio | 0.7484126984126984 | 0.13840846615052707 | hard voting |
| Woodblock_Woodblock_controls_sc_audio | 0.7503968253968254 | 0.11505473190108012 | hard voting |
| Bicycle_Bicycle_controls_sc_audio | 0.7511904761904762 | 0.13140614025282504 | knn |
| Rimshot_Rimshot_controls_sc_audio | 0.7521212121212122 | 0.0868518893790183 | logistic regression |
| Thememusic_Thememusic_controls_sc_audio | 0.7523809523809524 | 0.1547435886597326 | adaboost |
| Thunk_Thunk_controls_sc_audio | 0.7523809523809524 | 0.20198139830383138 | hard voting |
| Sitar_Sitar_controls_sc_audio | 0.7523809523809525 | 0.14394646411116996 | random forest |
| Rustlingleaves_Rustlingleaves_controls_sc_audio | 0.7531746031746033 | 0.06390737187046791 | logistic regression |
| Carpassingby_Carpassingby_controls_sc_audio | 0.7547619047619047 | 0.19374103413938368 | random forest |
| Pant_Pant_controls_sc_audio | 0.7555555555555555 | 0.1663564762739543 | knn |
| New-agemusic_New-agemusic_controls_sc_audio | 0.7559523809523809 | 0.0917516612761795 | gaussian-nb |
| Policecar(siren)_Policecar(siren)_controls_sc_audio | 0.7559523809523809 | 0.0917516612761795 | logistic regression |
| Stream_Stream_controls_sc_audio | 0.7559523809523809 | 0.1041921737478146 | logistic regression |
| Rain_Rain_controls_sc_audio | 0.7561904761904762 | 0.0957320523666976 | gaussian-nb |
| Gospelmusic_Gospelmusic_controls_sc_audio | 0.7567460317460318 | 0.09599238337971726 | gradient boosting |
| Turkey_Turkey_controls_sc_audio | 0.7567460317460318 | 0.1318248951186424 | random forest |
| Fowl_Fowl_controls_sc_audio | 0.7574615384615384 | 0.0764073480775029 | hard voting |
| Battlecry_Battlecry_controls_sc_audio | 0.7583333333333333 | 0.10341394704992381 | adaboost |
| Dancemusic_Dancemusic_controls_sc_audio | 0.7583333333333333 | 0.1522972240208089 | gaussian-nb |
| Fingersnapping_Fingersnapping_controls_sc_audio | 0.7583333333333333 | 0.17159383568311667 | hard voting |
| Sonar_Sonar_controls_sc_audio | 0.7583333333333333 | 0.1715938356831167 | logistic regression |
| Racecar,autoracing_Racecar,autoracing_controls_sc_audio | 0.759126984126984 | 0.16867460149416816 | decision-tree |
| Sewingmachine_Sewingmachine_controls_sc_audio | 0.7595238095238095 | 0.18760400659501222 | hard voting |
| Siren_Siren_controls_sc_audio | 0.76 | 0.09158692963776752 | gaussian-nb |
| Wind_Wind_controls_sc_audio | 0.7601731601731603 | 0.11686227167014779 | gaussian-nb |
| Motorvehicle(road)_Motorvehicle(road)_controls_sc_audio | 0.7607142857142858 | 0.1265717510476382 | gaussian-nb |
| Excitingmusic_Excitingmusic_controls_sc_audio | 0.7619047619047619 | 0.11313352178543148 | gaussian-nb |
| Firealarm_Firealarm_controls_sc_audio | 0.7626984126984127 | 0.17468252165321585 | gaussian-nb |
| Whimper_Whimper_controls_sc_audio | 0.7630952380952382 | 0.1778716447201882 | hard voting |
| Soundtrackmusic_Soundtrackmusic_controls_sc_audio | 0.7634920634920634 | 0.11112811661249035 | adaboost |
| Whalevocalization_Whalevocalization_controls_sc_audio | 0.7650793650793651 | 0.19216185333868643 | random forest |
| Vocalmusic_Vocalmusic_controls_sc_audio | 0.7662698412698413 | 0.12658916752369115 | hard voting |
| Cough_Cough_controls_sc_audio | 0.7666666666666666 | 0.09354143466934854 | random forest |
| Hands_Hands_controls_sc_audio | 0.7666666666666667 | 0.08579691784155835 | decision-tree |
| Jingle,tinkle_Jingle,tinkle_controls_sc_audio | 0.7666666666666667 | 0.08579691784155835 | gaussian-nb |
| MiddleEasternmusic_MiddleEasternmusic_controls_sc_audio | 0.7666666666666667 | 0.11666666666666667 | hard voting |
| Sailboat,sailingship_Sailboat,sailingship_controls_sc_audio | 0.7666666666666667 | 0.14092945437739804 | knn |
| Shuffle_Shuffle_controls_sc_audio | 0.7666666666666667 | 0.2306392083849675 | random forest |
| Croak_Croak_controls_sc_audio | 0.7670634920634921 | 0.09613991022525677 | adaboost |
| Rodents,rats,mice_Rodents,rats,mice_controls_sc_audio | 0.7682539682539682 | 0.15506888561041032 | knn |
| Acousticguitar_Acousticguitar_controls_sc_audio | 0.7682539682539683 | 0.08786255557522568 | adaboost |
| Mantra_Mantra_controls_sc_audio | 0.7682539682539683 | 0.08786255557522568 | knn |
| Wail,moan_Wail,moan_controls_sc_audio | 0.7682539682539683 | 0.11988068310158223 | logistic regression |
| Steamwhistle_Steamwhistle_controls_sc_audio | 0.7683333333333333 | 0.189212141703172 | gradient boosting |
| Doublebass_Doublebass_controls_sc_audio | 0.7690476190476191 | 0.06449603064733345 | hard voting |
| Filing(rasp)_Filing(rasp)_controls_sc_audio | 0.7690476190476191 | 0.11100902339622769 | random forest |
| Chime_Chime_controls_sc_audio | 0.7694444444444444 | 0.09686442096757053 | knn |
| Snoring_Snoring_controls_sc_audio | 0.7698412698412699 | 0.04807978168527287 | gaussian-nb |
| Waterfall_Waterfall_controls_sc_audio | 0.7698412698412699 | 0.04807978168527287 | knn |
| Writing_Writing_controls_sc_audio | 0.7698412698412699 | 0.1495773839922507 | random forest |
| Strum_Strum_controls_sc_audio | 0.7718253968253969 | 0.17715487528214058 | hard voting |
| Synthesizer_Synthesizer_controls_sc_audio | 0.7726190476190476 | 0.08095238095238094 | adaboost |
| Railroadcar,trainwagon_Railroadcar,trainwagon_controls_sc_audio | 0.7728695652173914 | 0.041544473630375355 | random forest |
| Electronicorgan_Electronicorgan_controls_sc_audio | 0.7734126984126984 | 0.12444383705715072 | knn |
| Disco_Disco_controls_sc_audio | 0.7746031746031745 | 0.17885163201273999 | knn |
| Funnymusic_Funnymusic_controls_sc_audio | 0.7746031746031746 | 0.07605808603625992 | gaussian-nb |
| Skateboard_Skateboard_controls_sc_audio | 0.7746031746031747 | 0.11810206500151287 | logistic regression |
| Theremin_Theremin_controls_sc_audio | 0.7746031746031747 | 0.11810206500151287 | logistic regression |
| Beep,bleep_Beep,bleep_controls_sc_audio | 0.775 | 0.07264831572567791 | hard voting |
| Caterwaul_Caterwaul_controls_sc_audio | 0.775 | 0.07264831572567791 | knn |
| Folkmusic_Folkmusic_controls_sc_audio | 0.775 | 0.1457737973711325 | knn |
| Throatclearing_Throatclearing_controls_sc_audio | 0.775 | 0.1457737973711325 | random forest |
| Whistling_Whistling_controls_sc_audio | 0.775 | 0.1457737973711325 | sk |
| Distortion_Distortion_controls_sc_audio | 0.7753968253968253 | 0.11086565859399372 | logistic regression |
| Malesinging_Malesinging_controls_sc_audio | 0.7753968253968254 | 0.08457502733179185 | knn |
| Musicforchildren_Musicforchildren_controls_sc_audio | 0.7777777777777778 | 0.11962821385026522 | gaussian-nb |
| Telephonebellringing_Telephonebellringing_controls_sc_audio | 0.7777777777777778 | 0.19697894676175962 | gradient boosting |
| Clatter_Clatter_controls_sc_audio | 0.7781746031746033 | 0.08015873015873015 | gaussian-nb |
| Chainsaw_Chainsaw_controls_sc_audio | 0.778968253968254 | 0.08477215917996458 | gaussian-nb |
| Steam_Steam_controls_sc_audio | 0.778968253968254 | 0.14243544461647872 | random forest |
| Cupboardopenorclose_Cupboardopenorclose_controls_sc_audio | 0.7797619047619048 | 0.1357351696546593 | knn |
| Wheeze_Wheeze_controls_sc_audio | 0.7797619047619048 | 0.1357351696546593 | logistic regression |
| Coin(dropping)_Coin(dropping)_controls_sc_audio | 0.7797619047619049 | 0.0855156428384189 | logistic regression |
| Keyboard(musical)_Keyboard(musical)_controls_sc_audio | 0.7802889576883385 | 0.11736718289193313 | hard voting |
| Ambientmusic_Ambientmusic_controls_sc_audio | 0.780952380952381 | 0.11427331281920437 | decision-tree |
| Birdflight,flappingwings_Birdflight,flappingwings_controls_sc_audio | 0.7809523809523811 | 0.11681504439983552 | adaboost |
| Scratching(performancetechnique)_Scratching(performancetechnique)_controls_sc_audio | 0.7809523809523811 | 0.1476787726934985 | knn |
| Squawk_Squawk_controls_sc_audio | 0.7809523809523811 | 0.1476787726934985 | random forest |
| Trainwhistle_Trainwhistle_controls_sc_audio | 0.7817460317460319 | 0.11528443687566628 | random forest |
| Crushing_Crushing_controls_sc_audio | 0.7825396825396825 | 0.08052329481467167 | adaboost |
| Mediumengine(midfrequency)_Mediumengine(midfrequency)_controls_sc_audio | 0.7825396825396825 | 0.1629286021632551 | decision-tree |
| Trainhorn_Trainhorn_controls_sc_audio | 0.7825396825396825 | 0.16597835950094622 | gaussian-nb |
| Flamenco_Flamenco_controls_sc_audio | 0.7841269841269842 | 0.14289241187208762 | gaussian-nb |
| Powertool_Powertool_controls_sc_audio | 0.7842424242424243 | 0.08277800888659415 | knn |
| Canidae,dogs,wolves_Canidae,dogs,wolves_controls_sc_audio | 0.7845238095238095 | 0.1321589436797897 | adaboost |
| Accordion_Accordion_controls_sc_audio | 0.7857142857142857 | 0.16170330603816818 | knn |
| Choruseffect_Choruseffect_controls_sc_audio | 0.7880952380952382 | 0.036161224602839714 | gradient boosting |
| Cricket_Cricket_controls_sc_audio | 0.7880952380952382 | 0.14512312215677453 | logistic regression |
| Tapping(guitartechnique)_Tapping(guitartechnique)_controls_sc_audio | 0.7884920634920635 | 0.19663329078669112 | logistic regression |
| Bathtub(fillingorwashing)_Bathtub(fillingorwashing)_controls_sc_audio | 0.7892857142857143 | 0.1815466432448405 | decision-tree |
| Jazz_Jazz_controls_sc_audio | 0.7892857142857144 | 0.17068290207640743 | logistic regression |
| Chant_Chant_controls_sc_audio | 0.7904761904761906 | 0.07197323205558495 | decision-tree |
| Crack_Crack_controls_sc_audio | 0.7904761904761906 | 0.07197323205558495 | gaussian-nb |
| Gargling_Gargling_controls_sc_audio | 0.7904761904761906 | 0.07197323205558495 | hard voting |
| Rockandroll_Rockandroll_controls_sc_audio | 0.7904761904761906 | 0.07197323205558495 | hard voting |
| Shofar_Shofar_controls_sc_audio | 0.7904761904761906 | 0.08302664654363186 | hard voting |
| Throbbing_Throbbing_controls_sc_audio | 0.7904761904761906 | 0.11551368507085874 | hard voting |
| Trancemusic_Trancemusic_controls_sc_audio | 0.7904761904761906 | 0.11551368507085874 | logistic regression |
| Trickle,dribble_Trickle,dribble_controls_sc_audio | 0.7904761904761906 | 0.1227057021592869 | logistic regression |
| Vacuumcleaner_Vacuumcleaner_controls_sc_audio | 0.7904761904761906 | 0.1227057021592869 | logistic regression |
| Whistle_Whistle_controls_sc_audio | 0.7904761904761906 | 0.1523809523809524 | random forest |
| Hammondorgan_Hammondorgan_controls_sc_audio | 0.7911111111111111 | 0.1451095797094623 | hard voting |
| Cello_Cello_controls_sc_audio | 0.7916666666666666 | 0.09702360664762764 | random forest |
| Raindrop_Raindrop_controls_sc_audio | 0.7944444444444445 | 0.12589187992916287 | knn |
| Chuckle,chortle_Chuckle,chortle_controls_sc_audio | 0.7964285714285715 | 0.12555997022319249 | logistic regression |
| Foghorn_Foghorn_controls_sc_audio | 0.7968253968253968 | 0.1556527069476986 | knn |
| Flute_Flute_controls_sc_audio | 0.7968253968253969 | 0.08888888888888886 | knn |
| Knock_Knock_controls_sc_audio | 0.7968253968253969 | 0.08888888888888886 | logistic regression |
| Windchime_Windchime_controls_sc_audio | 0.7968253968253969 | 0.12674580811223574 | logistic regression |
| Cymbal_Cymbal_controls_sc_audio | 0.7972222222222223 | 0.1277777777777778 | gaussian-nb |
| Flap_Flap_controls_sc_audio | 0.7984126984126985 | 0.09301810767129862 | decision-tree |
| Smokedetector,smokealarm_Smokedetector,smokealarm_controls_sc_audio | 0.7984126984126985 | 0.18858853003529072 | logistic regression |
| Beatboxing_Beatboxing_controls_sc_audio | 0.8 | 0.04844521416518047 | adaboost |
| Bowedstringinstrument_Bowedstringinstrument_controls_sc_audio | 0.8 | 0.1274754878398196 | hard voting |
| Ding_Ding_controls_sc_audio | 0.8 | 0.1274754878398196 | hard voting |
| Hubbub,speechnoise,speechbabble_Hubbub,speechnoise,speechbabble_controls_sc_audio | 0.8 | 0.12747548783981963 | logistic regression |
| Scratch_Scratch_controls_sc_audio | 0.8 | 0.1695582495781317 | logistic regression |
| Techno_Techno_controls_sc_audio | 0.8 | 0.19378085666072192 | logistic regression |
| Zither_Zither_controls_sc_audio | 0.8003968253968253 | 0.15230859723977136 | gradient boosting |
| Gong_Gong_controls_sc_audio | 0.8031746031746032 | 0.11733154674651639 | logistic regression |
| Yip_Yip_controls_sc_audio | 0.8031746031746032 | 0.1537635687404741 | random forest |
| Drill_Drill_controls_sc_audio | 0.803968253968254 | 0.08322366177091002 | adaboost |
| Weddingmusic_Weddingmusic_controls_sc_audio | 0.803968253968254 | 0.1729284765430381 | gradient boosting |
| Electronicmusic_Electronicmusic_controls_sc_audio | 0.8047619047619048 | 0.12358954817149206 | knn |
| Lullaby_Lullaby_controls_sc_audio | 0.8047619047619048 | 0.13941284389568956 | logistic regression |
| Grunt_Grunt_controls_sc_audio | 0.8063492063492064 | 0.14869890068102057 | hard voting |
| Ska_Ska_controls_sc_audio | 0.8063492063492064 | 0.14869890068102057 | random forest |
| Bassguitar_Bassguitar_controls_sc_audio | 0.8075396825396826 | 0.18620373706142745 | gradient boosting |
| Sneeze_Sneeze_controls_sc_audio | 0.8076190476190476 | 0.11670456138697441 | adaboost |
| Thunder_Thunder_controls_sc_audio | 0.8083333333333332 | 0.10628403594282772 | gaussian-nb |
| Electronica_Electronica_controls_sc_audio | 0.8083333333333333 | 0.05 | adaboost |
| Malespeech,manspeaking_Malespeech,manspeaking_controls_sc_audio | 0.8083333333333333 | 0.11666666666666668 | gaussian-nb |
| MusicofAfrica_MusicofAfrica_controls_sc_audio | 0.8083333333333333 | 0.14092945437739804 | gradient boosting |
| Videogamemusic_Videogamemusic_controls_sc_audio | 0.8083333333333333 | 0.16158932858054434 | logistic regression |
| Truck_Truck_controls_sc_audio | 0.8084848484848484 | 0.11584163218185627 | adaboost |
| Ukulele_Ukulele_controls_sc_audio | 0.8095238095238095 | 0.15649215928719032 | gaussian-nb |
| Singingbowl_Singingbowl_controls_sc_audio | 0.8103174603174603 | 0.15025802951795383 | gaussian-nb |
| Reggae_Reggae_controls_sc_audio | 0.8107142857142857 | 0.11157499537009506 | adaboost |
| Railtransport_Railtransport_controls_sc_audio | 0.8123333333333334 | 0.0442919606449949 | random forest |
| Biting_Biting_controls_sc_audio | 0.8126984126984127 | 0.08118547207964709 | adaboost |
| Heavymetal_Heavymetal_controls_sc_audio | 0.8126984126984127 | 0.12146746964894596 | gaussian-nb |
| Psychedelicrock_Psychedelicrock_controls_sc_audio | 0.8126984126984127 | 0.1669008181345386 | logistic regression |
| Hiphopmusic_Hiphopmusic_controls_sc_audio | 0.8134920634920635 | 0.11330042650630427 | random forest |
| Electricguitar_Electricguitar_controls_sc_audio | 0.8138888888888889 | 0.11439589045541113 | hard voting |
| Glockenspiel_Glockenspiel_controls_sc_audio | 0.8138888888888889 | 0.1599575560987552 | logistic regression |
| Stir_Stir_controls_sc_audio | 0.8162698412698413 | 0.10907718921643064 | gaussian-nb |
| Rumble_Rumble_controls_sc_audio | 0.8166666666666667 | 0.12527746981977425 | hard voting |
| Hiccup_Hiccup_controls_sc_audio | 0.817063492063492 | 0.07096853620986715 | logistic regression |
| Jackhammer_Jackhammer_controls_sc_audio | 0.817063492063492 | 0.07096853620986715 | random forest |
| Chopping(food)_Chopping(food)_controls_sc_audio | 0.8178571428571428 | 0.12494896917525643 | logistic regression |
| Airbrake_Airbrake_controls_sc_audio | 0.819047619047619 | 0.11070219539150916 | gradient boosting |
| Electronictuner_Electronictuner_controls_sc_audio | 0.819047619047619 | 0.17405397030949588 | knn |
| Toothbrush_Toothbrush_controls_sc_audio | 0.819047619047619 | 0.21191516531147475 | random forest |
| Electronicdancemusic_Electronicdancemusic_controls_sc_audio | 0.8194444444444444 | 0.11180339887498948 | knn |
| Typing_Typing_controls_sc_audio | 0.8194444444444444 | 0.11180339887498948 | logistic regression |
| Popmusic_Popmusic_controls_sc_audio | 0.8198412698412698 | 0.1473628088429477 | adaboost |
| Gobble_Gobble_controls_sc_audio | 0.8206349206349206 | 0.05882660463557592 | logistic regression |
| Tendermusic_Tendermusic_controls_sc_audio | 0.8206349206349206 | 0.10781388926790839 | logistic regression |
| Train_Train_controls_sc_audio | 0.8220000000000001 | 0.0769805170156709 | knn |
| Fusillade_Fusillade_controls_sc_audio | 0.8234126984126984 | 0.12239989147917732 | random forest |
| Laughter_Laughter_controls_sc_audio | 0.8238095238095238 | 0.07158712561129957 | gradient boosting |
| Crumpling,crinkling_Crumpling,crinkling_controls_sc_audio | 0.8242063492063492 | 0.16962417515251274 | logistic regression |
| Organ_Organ_controls_sc_audio | 0.8245098039215687 | 0.07663083386074433 | gradient boosting |
| Backgroundmusic_Backgroundmusic_controls_sc_audio | 0.825 | 0.1695582495781317 | decision-tree |
| Drumandbass_Drumandbass_controls_sc_audio | 0.825 | 0.18708286933869706 | knn |
| Honk_Honk_controls_sc_audio | 0.8253968253968254 | 0.03888078956798692 | decision-tree |
| Maraca_Maraca_controls_sc_audio | 0.8253968253968254 | 0.09836148180844233 | gradient boosting |
| Syntheticsinging_Syntheticsinging_controls_sc_audio | 0.8253968253968254 | 0.12088528739466521 | hard voting |
| Vibraphone_Vibraphone_controls_sc_audio | 0.8253968253968254 | 0.12088528739466521 | hard voting |
| Walk,footsteps_Walk,footsteps_controls_sc_audio | 0.8253968253968254 | 0.1715461090299212 | hard voting |
| Fieldrecording_Fieldrecording_controls_sc_audio | 0.8261904761904761 | 0.052907407341266505 | gaussian-nb |
| Fill(withliquid)_Fill(withliquid)_controls_sc_audio | 0.8261904761904761 | 0.10470176243835226 | logistic regression |
| Howl_Howl_controls_sc_audio | 0.8261904761904761 | 0.144357203725944 | logistic regression |
| Choir_Choir_controls_sc_audio | 0.8269841269841269 | 0.10166322807463274 | adaboost |
| Whoop_Whoop_controls_sc_audio | 0.8269841269841269 | 0.12358674503154887 | decision-tree |
| Aircraftengine_Aircraftengine_controls_sc_audio | 0.8285714285714285 | 0.1665986255670086 | logistic regression |
| Buzzer_Buzzer_controls_sc_audio | 0.8285714285714285 | 0.20995626366712958 | logistic regression |
| Frenchhorn_Frenchhorn_controls_sc_audio | 0.8289682539682539 | 0.0423024062578934 | gaussian-nb |
| Grunge_Grunge_controls_sc_audio | 0.8289682539682539 | 0.17235383750031036 | logistic regression |
| Bluegrass_Bluegrass_controls_sc_audio | 0.8297619047619047 | 0.11378860138427163 | adaboost |
| Tick_Tick_controls_sc_audio | 0.8297619047619047 | 0.12478502552434774 | logistic regression |
| Violin,fiddle_Violin,fiddle_controls_sc_audio | 0.8297619047619047 | 0.12478502552434774 | random forest |
| Windnoise(microphone)_Windnoise(microphone)_controls_sc_audio | 0.8298245614035089 | 0.10604646823438048 | adaboost |
| Sink(fillingorwashing)_Sink(fillingorwashing)_controls_sc_audio | 0.8305555555555555 | 0.09638528651609707 | logistic regression |
| Blues_Blues_controls_sc_audio | 0.8317460317460317 | 0.10932809750934963 | logistic regression |
| Speechsynthesizer_Speechsynthesizer_controls_sc_audio | 0.8317460317460318 | 0.14183052637262653 | decision-tree |
| Christianmusic_Christianmusic_controls_sc_audio | 0.8325396825396825 | 0.09105910799532359 | gradient boosting |
| Waves,surf_Waves,surf_controls_sc_audio | 0.8325396825396825 | 0.11502187945709405 | logistic regression |
| Babbling_Babbling_controls_sc_audio | 0.8333333333333334 | 0.045643546458763846 | gaussian-nb |
| Funk_Funk_controls_sc_audio | 0.8333333333333334 | 0.12076147288491199 | random forest |
| Shatter_Shatter_controls_sc_audio | 0.834920634920635 | 0.1681640969923686 | gaussian-nb |
| Heavyengine(lowfrequency)_Heavyengine(lowfrequency)_controls_sc_audio | 0.8357142857142857 | 0.10914790564240089 | gaussian-nb |
| Soulmusic_Soulmusic_controls_sc_audio | 0.8357142857142857 | 0.1622545241657221 | gaussian-nb |
| Drumkit_Drumkit_controls_sc_audio | 0.8358974358974359 | 0.07471180658632545 | logistic regression |
| Jetengine_Jetengine_controls_sc_audio | 0.836111111111111 | 0.11600340565456167 | random forest |
| Alarmclock_Alarmclock_controls_sc_audio | 0.8384920634920634 | 0.11028319668883052 | gaussian-nb |
| Dialtone_Dialtone_controls_sc_audio | 0.8384920634920634 | 0.14256804963956593 | logistic regression |
| Sniff_Sniff_controls_sc_audio | 0.8388888888888889 | 0.13653561919382787 | knn |
| Childsinging_Childsinging_controls_sc_audio | 0.8412698412698412 | 0.21224780508503846 | gradient boosting |
| Crunch_Crunch_controls_sc_audio | 0.8412698412698413 | 0.09576573415237051 | knn |
| Dubstep_Dubstep_controls_sc_audio | 0.8412698412698413 | 0.09576573415237051 | logistic regression |
| Clang_Clang_controls_sc_audio | 0.8416666666666666 | 0.0927960727138337 | hard voting |
| Hairdryer_Hairdryer_controls_sc_audio | 0.8416666666666666 | 0.12190615698606495 | sk |
| Patter_Patter_controls_sc_audio | 0.8420634920634921 | 0.06467888781199489 | knn |
| Applause_Applause_controls_sc_audio | 0.8448412698412697 | 0.06631141173112477 | adaboost |
| Motorboat,speedboat_Motorboat,speedboat_controls_sc_audio | 0.8448412698412697 | 0.0966202614916407 | gaussian-nb |
| Rapping_Rapping_controls_sc_audio | 0.8448412698412697 | 0.16019365013307466 | gaussian-nb |
| Harpsichord_Harpsichord_controls_sc_audio | 0.8456349206349205 | 0.04928309427384133 | gaussian-nb |
| Banjo_Banjo_controls_sc_audio | 0.8476190476190476 | 0.03702191679266855 | gaussian-nb |
| Bicyclebell_Bicyclebell_controls_sc_audio | 0.8476190476190476 | 0.03702191679266855 | gaussian-nb |
| Frying(food)_Frying(food)_controls_sc_audio | 0.8476190476190476 | 0.09764162856653777 | gradient boosting |
| Sadmusic_Sadmusic_controls_sc_audio | 0.8476190476190476 | 0.09764162856653777 | knn |
| Swingmusic_Swingmusic_controls_sc_audio | 0.8476190476190476 | 0.09764162856653777 | logistic regression |
| Cashregister_Cashregister_controls_sc_audio | 0.8484126984126984 | 0.036209094347683775 | gaussian-nb |
| Static_Static_controls_sc_audio | 0.8484126984126984 | 0.1253968253968254 | logistic regression |
| Stringsection_Stringsection_controls_sc_audio | 0.8492063492063492 | 0.09387248444487266 | hard voting |
| Heartmurmur_Heartmurmur_controls_sc_audio | 0.85 | 0.09354143466934853 | hard voting |
| Punkrock_Punkrock_controls_sc_audio | 0.85 | 0.09354143466934853 | hard voting |
| Crowd_Crowd_controls_sc_audio | 0.8505847953216374 | 0.07560930863596947 | gradient boosting |
| Happymusic_Happymusic_controls_sc_audio | 0.851190476190476 | 0.03859624258980262 | gaussian-nb |
| Purr_Purr_controls_sc_audio | 0.8539682539682539 | 0.10737482238277947 | hard voting |
| Splinter_Splinter_controls_sc_audio | 0.8539682539682539 | 0.10737482238277947 | random forest |
| Accelerating,revving,vroom_Accelerating,revving,vroom_controls_sc_audio | 0.8547619047619047 | 0.08850540863143269 | gaussian-nb |
| Clickety-clack_Clickety-clack_controls_sc_audio | 0.8551515151515151 | 0.05493166674539744 | adaboost |
| Yell_Yell_controls_sc_audio | 0.8575396825396826 | 0.10771744810780727 | hard voting |
| Pizzicato_Pizzicato_controls_sc_audio | 0.8583333333333332 | 0.07961617026648063 | gradient boosting |
| Effectsunit_Effectsunit_controls_sc_audio | 0.8589010989010989 | 0.05966779991804236 | adaboost |
| Bouncing_Bouncing_controls_sc_audio | 0.8603174603174603 | 0.1629286021632551 | hard voting |
| Ratchet,pawl_Ratchet,pawl_controls_sc_audio | 0.8603174603174603 | 0.1629286021632551 | logistic regression |
| Cheering_Cheering_controls_sc_audio | 0.861111111111111 | 0.10794088459847472 | logistic regression |
| Engine_Engine_controls_sc_audio | 0.8616666666666667 | 0.020602049520483258 | hard voting |
| Bellylaugh_Bellylaugh_controls_sc_audio | 0.8630952380952381 | 0.08074202360863414 | random forest |
| Groan_Groan_controls_sc_audio | 0.8634920634920634 | 0.09123878008380898 | adaboost |
| Humming_Humming_controls_sc_audio | 0.8634920634920634 | 0.09123878008380898 | logistic regression |
| Thunderstorm_Thunderstorm_controls_sc_audio | 0.8638888888888889 | 0.16301556390134678 | gaussian-nb |
| Arrow_Arrow_controls_sc_audio | 0.8666666666666666 | 0.08079466429027216 | adaboost |
| Busysignal_Busysignal_controls_sc_audio | 0.8666666666666666 | 0.08079466429027216 | gradient boosting |
| Whimper(dog)_Whimper(dog)_controls_sc_audio | 0.8666666666666666 | 0.1130388330520878 | logistic regression |
| Opera_Opera_controls_sc_audio | 0.8670634920634921 | 0.09126984126984125 | adaboost |
| Propeller,airscrew_Propeller,airscrew_controls_sc_audio | 0.8670634920634921 | 0.15702456666925377 | hard voting |
| Crowing,cock-a-doodle-doo_Crowing,cock-a-doodle-doo_controls_sc_audio | 0.8678571428571429 | 0.12037356818823369 | logistic regression |
| Civildefensesiren_Civildefensesiren_controls_sc_audio | 0.8698412698412697 | 0.11551368507085874 | adaboost |
| Fireengine,firetruck(siren)_Fireengine,firetruck(siren)_controls_sc_audio | 0.8698412698412697 | 0.11551368507085874 | gaussian-nb |
| Subway,metro,underground_Subway,metro,underground_controls_sc_audio | 0.86984126984127 | 0.09167954970281683 | adaboost |
| Environmentalnoise_Environmentalnoise_controls_sc_audio | 0.8706349206349205 | 0.12066624488887003 | gradient boosting |
| Ocean_Ocean_controls_sc_audio | 0.8711111111111112 | 0.07875575620741931 | decision-tree |
| Salsamusic_Salsamusic_controls_sc_audio | 0.8714285714285716 | 0.11203133672398659 | gaussian-nb |
| Aircraft_Aircraft_controls_sc_audio | 0.8733333333333334 | 0.08305941375396247 | random forest |
| Babylaughter_Babylaughter_controls_sc_audio | 0.875 | 0.11180339887498948 | gradient boosting |
| Bagpipes_Bagpipes_controls_sc_audio | 0.875 | 0.11180339887498948 | knn |
| Doorbell_Doorbell_controls_sc_audio | 0.875 | 0.13693063937629152 | random forest |
| Roll_Roll_controls_sc_audio | 0.8761904761904761 | 0.11551368507085874 | gradient boosting |
| Clarinet_Clarinet_controls_sc_audio | 0.8769841269841269 | 0.07124093520638519 | gaussian-nb |
| Idling_Idling_controls_sc_audio | 0.8769841269841269 | 0.07124093520638519 | knn |
| Heartsounds,heartbeat_Heartsounds,heartbeat_controls_sc_audio | 0.8827777777777778 | 0.07970625081982645 | gradient boosting |
| Trombone_Trombone_controls_sc_audio | 0.8827777777777778 | 0.13730654179518573 | logistic regression |
| Harp_Harp_controls_sc_audio | 0.8833333333333332 | 0.10599324460188285 | gaussian-nb |
| Sidetone_Sidetone_controls_sc_audio | 0.8857142857142858 | 0.10690449676496976 | logistic regression |
| Chewing,mastication_Chewing,mastication_controls_sc_audio | 0.8916666666666666 | 0.0565194165260439 | knn |
| Silence_Silence_controls_sc_audio | 0.8916666666666666 | 0.097182531580755 | logistic regression |
| Conversation_Conversation_controls_sc_audio | 0.8928571428571429 | 0.13170777796132696 | logistic regression |
| Bassdrum_Bassdrum_controls_sc_audio | 0.8933333333333333 | 0.07039570693980955 | logistic regression |
| Computerkeyboard_Computerkeyboard_controls_sc_audio | 0.8956349206349206 | 0.05352878961561032 | gradient boosting |
| Engineknocking_Engineknocking_controls_sc_audio | 0.8956349206349206 | 0.10501712538359978 | logistic regression |
| Sampler_Sampler_controls_sc_audio | 0.8956349206349206 | 0.10501712538359978 | random forest |
| Sigh_Sigh_controls_sc_audio | 0.8964285714285716 | 0.09476070829586856 | gradient boosting |
| Tuningfork_Tuningfork_controls_sc_audio | 0.8964285714285716 | 0.14655917520487993 | knn |
| Bark_Bark_controls_sc_audio | 0.8984126984126984 | 0.0878625555752257 | adaboost |
| Trafficnoise,roadwaynoise_Trafficnoise,roadwaynoise_controls_sc_audio | 0.8984126984126984 | 0.0878625555752257 | logistic regression |
| Angrymusic_Angrymusic_controls_sc_audio | 0.8992063492063492 | 0.09429426501764536 | adaboost |
| Orchestra_Orchestra_controls_sc_audio | 0.9 | 0.09354143466934853 | gaussian-nb |
| Sinewave_Sinewave_controls_sc_audio | 0.9019841269841269 | 0.08646423827151908 | knn |
| Lightengine(highfrequency)_Lightengine(highfrequency)_controls_sc_audio | 0.9047619047619048 | 0.13127665478181164 | random forest |
| Trainwheelssquealing_Trainwheelssquealing_controls_sc_audio | 0.9055555555555556 | 0.11600340565456166 | gaussian-nb |
| Progressiverock_Progressiverock_controls_sc_audio | 0.9083333333333332 | 0.08407081083567532 | knn |
| Clicking_Clicking_controls_sc_audio | 0.9142857142857143 | 0.06998542122237654 | gaussian-nb |
| Eruption_Eruption_controls_sc_audio | 0.9142857142857143 | 0.11428571428571428 | gradient boosting |
| Whispering_Whispering_controls_sc_audio | 0.9142857142857143 | 0.11428571428571428 | knn |
| Narration,monologue_Narration,monologue_controls_sc_audio | 0.9166666666666666 | 0.10540925533894598 | hard voting |
| Breaking_Breaking_controls_sc_audio | 0.9206349206349206 | 0.11178931340735879 | decision-tree |
| Whir_Whir_controls_sc_audio | 0.9206349206349206 | 0.11178931340735879 | logistic regression |
| Childrenshouting_Childrenshouting_controls_sc_audio | 0.9214285714285715 | 0.10202040612204072 | logistic regression |
| Fixed-wingaircraft,airplane_Fixed-wingaircraft,airplane_controls_sc_audio | 0.9242063492063493 | 0.06269841269841271 | gaussian-nb |
| Scarymusic_Scarymusic_controls_sc_audio | 0.9242063492063493 | 0.06269841269841271 | logistic regression |
| Tearing_Tearing_controls_sc_audio | 0.9269841269841269 | 0.06073373482447301 | gaussian-nb |
| Hi-hat_Hi-hat_controls_sc_audio | 0.9277777777777778 | 0.059186877090729215 | hard voting |
| Plop_Plop_controls_sc_audio | 0.9416666666666667 | 0.07264831572567787 | gradient boosting |
| Rhythmandblues_Rhythmandblues_controls_sc_audio | 0.9428571428571428 | 0.11428571428571428 | adaboost |
| Afrobeat_Afrobeat_controls_sc_audio | 0.9492063492063492 | 0.06301407378183878 | logistic regression |
| Changeringing(campanology)_Changeringing(campanology)_controls_sc_audio | 0.9555555555555555 | 0.054433105395181765 | adaboost |
| Dishes,pots,andpans_Dishes,pots,andpans_controls_sc_audio | 0.9555555555555555 | 0.054433105395181765 | hard voting |
| MusicofAsia_MusicofAsia_controls_sc_audio | 0.9555555555555555 | 0.08888888888888889 | random forest |
| Capgun_Capgun_controls_sc_audio | 0.975 | 0.049999999999999996 | logistic regression |
| Boom_Boom_controls_sc_audio | 0.9777777777777779 | 0.04444444444444447 | logistic regression |

## references
* Audioset. https://research.google.com/audioset/
