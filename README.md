# CanSat-2026-Project-Pliocene

Notes from Brian: 11/3/26
* PID to control the gimbal (controlled by the microcontroller mounted by the camera); board on camera needs high-freq gyro
* Should gimbal control tilt as well? Or will the parachute handle it?
* Flywheel stabilizes the device? Gimbal mount is coupled to parachute, boom and solar panels can spin as they wish
* Need to control rotation of parachute (not too fast)
* Microcontroller must be able to communicate with main board to be able to turn camera manually from ground station command
* ASCII data from PQ down to ground station, which will receive and parse it
* Data sent through ESP32 on PQ and container to groundstation

To-Do:
* First task: get communication functional through ESP32s using ESPNOW
* Get familiar with ESP32s programming and general arduino construction
* Look into mini cameras
- [ex1](https://www.amazon.com/Arducam-IMX219-Autofocus-Camera-Module/dp/B0GS5814J8/ref=sr_1_1_sspa?dib=eyJ2IjoiMSJ9.R9CFnBfsEhexcuiPrIiIHHjgc-R9uWMhXXQJwdWWKfRzVp0GzO0LIS9nEJdPXbfT11Q6gNJz4b0-TAFwgTor71g5vL76AMu17VOL5VfF_jMPQ64VjRovIY30IcExEEPUGwUoS9F08QRdpE1If0CFStHZlyy2aEvC86FBblf7X3gilbxpdElBJoDENaQlpR0BOWU0zS3XP_Px6TDbj5uR9fDquv1FWRxEccgdyHHtrWE.c9oXvtzA9WPd1O-4QNhhxQFEc0bWXNYFq8QN2klfEWc&dib_tag=se&keywords=mini+camera+module&qid=1793719609&sr=8-1-spons&sp_csd=d2lkZ2V0TmFtZT1zcF9hdGY&psc=1)
- [ex2](https://www.amazon.com/Inno-Maker-Camera-Module-OV5647-Raspberry/dp/B07G9VLPZH/ref=sxin_15_pa_sp_search_thematic_sspa?content-id=amzn1.sym.f97776bc-458f-4c8b-b734-d80b5430252e%3Aamzn1.sym.f97776bc-458f-4c8b-b734-d80b5430252e&cv_ct_cx=mini+camera+module&keywords=mini+camera+module&pd_rd_i=B07G9VLPZH&pd_rd_r=4be13433-8512-44f6-bd5f-df9f571f83ac&pd_rd_w=XDeQv&pd_rd_wg=dSPGS&pf_rd_p=f97776bc-458f-4c8b-b734-d80b5430252e&pf_rd_r=6RQPRZQR3MAP544FGKHW&qid=1793719609&sbo=RZvfv%2F%2FHxDF%2BO5021pAnSA%3D%3D&sr=1-2-6024b2a3-78e4-4fed-8fed-e1613be3bcce-spons&aref=V4Gjibvt2i&sp_csd=d2lkZ2V0TmFtZT1zcF9zZWFyY2hfdGhlbWF0aWM&psc=1)
- [ex3](https://www.amazon.com/dp/B0CLRN9QRC/ref=sspa_dk_detail_0?psc=1&pd_rd_i=B0CLRN9QRC&pd_rd_w=94ONI&content-id=amzn1.sym.4a7f44df-467c-45a1-af5f-91661a6df2f9&pf_rd_p=4a7f44df-467c-45a1-af5f-91661a6df2f9&pf_rd_r=40AW5AVADTAVSKB94680&pd_rd_wg=cFGbW&pd_rd_r=86370ecb-58d5-4f71-8d6d-f6254b847bb3&sp_csd=d2lkZ2V0TmFtZT1zcF9kZXRhaWwy)
