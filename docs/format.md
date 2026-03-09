```
[
  {
    "img_path": "n02085782-Japanese_spaniel/n02085782_2886.jpg",
    "img_width": 350,
    "img_height": 272,
    "img_bbox": [ 205, 20, 116, 201 ],
    "is_multiple_dogs": false,
    "joints": [
      [ 108.6, 252, 1 ],
      [ 147.6, 229, 1 ],
      [ 163.5, 208.5, 1 ],
      [ 0, 0, 0 ],
      [ 0, 0, 0 ],
      [ 0, 0, 0 ],
      [ 54, 244, 1 ],
      [ 77.4, 225.3, 1 ],
      [ 79, 196.5, 1 ],
      [ 0, 0, 0 ],
      [ 0, 0, 0 ],
      [ 0, 0, 0 ],
      [ 0, 0, 0 ],
      [ 0, 0, 0 ],
      [ 150.6, 86.6, 1 ],
      [ 88.7, 73, 1 ],
      [ 116, 106.3, 1 ],
      [ 109, 123.3, 1 ],
      [ 0, 0, 0 ],
      [ 0, 0, 0 ],
      [ 0, 0, 0 ],
      [ 0, 0, 0 ],
      [ 0, 0, 0 ],
      [ 0, 0, 0 ]
    ],
    "seg": "Yi71c01S74jHNU75gHMX75eHM[74cHM\\76`HL4HQ7k0lHXOT7R1O2N010O010jLiNROW1m0lNROT1m0oNPOQ1P1QOoNn0R1ROnNn0oMkNQ2:Nl0oMlNQ2:0j0nMnNP291j0mMoNR280j0kMPOLEg1c0`0i0lMCb1Db0i0jMGa1Ae0h0iMI`1_Og0j0fMK`1\\Oj0i0eMN^1ZOl0i0dM1]1WOm0k0cM2]1TOP1j0bM4\\1ROR1k0`M<W1iNX1l0`M=:ZN4=Q2T3aMXLO8>=Q2k3oMULQ2k3oMTLQ2m3mMULS2j3mMWLS2i3kMYLT2h3kMYLU2f3lMYLT2h3jMYLV2i3hMXLW2j3dMZL\\2k42O1O100O1O1O100O1O1O2N1N2N2O1N2OdMfJd1X5[NkJe1T5ZNoJe1Q5YNQKh1n4WNTKh1l4VNVKj1j4VNWKi1i4WNXKh1h4WNYKi1g4WNZKh1f4XNZKh1g4VNZKj1f4UN[Kl1d4TN\\Kl1d4SN]Km1c4SN]Km1d4QN]Ko1c4QN^Kn1b4QN_Ko1a4QN_Ko1a4QN_KP2a4nM`KR2`4nM`KR2_4nMbKR2^4nMbKR2^4nMbKR2^4mMcKS2]4mMcKT2[4lMeKU2[4kMeKU2[4jMfKV2Z4jMfKV2Z4iMfKY2X4hMhKX2X4gMhKZ2X4fMhKZ2X4eMgK^2X4bMgK_2X4aMhK`2X4`MgKa2S52M2O1O1O2O0000001O1O000O1000001N1000000O100O2O0O100O101N1O101N100O2O001N101N101N2O0O2O0O2N2O0O2N101N2N101N101M4N1O2AlKZLY4e3:01M2Ma0]O4I8L3J8M2O2NM310O01NI8J6K5K5K5J6N2O1J6G9M3K5I7ChK_L]4_3eK^L\\4a3;M4L3N2N3M1nLjJi2`5N7J1N2N101O1O1O1O1N101N100000O10O010000O100O1000000O1O1BlM`JT2`5>O1IYMdJh2\\56O100O10001N1N21O01O0013M;D10O1O001O01O2N00100O2N01O0010O01O1O00001O0O2O1N1O100J6\\Od000O010O100O2O0N3L3L5iMlKLX42mKFY48jKA[4>\\L_NU4Z1g1H5K5M3N1N2O1N4M2M3N1M4L9G7IbY6"
  },
]
```

# Dog Keypoints Visualization
This notebook loads dog images from the Stanford Dogs dataset and displays the annotated keypoints.

## Keypoints Legend:
The dataset uses 24 keypoints for dog pose estimation:

**Legs**
- 0: Front Left Paw
- 1: Front Left Knee
- 2: Front Left Elbow
- 3: Rear Left Paw
- 4: Rear Left Knee
- 5: Rear Left Elbow
- 6: Front Right Paw
- 7: Front Right Knee
- 8: Front Right Elbow
- 9: Rear Right Paw
- 10: Rear Right Knee
- 11: Rear Right Elbow

**Body:**
- 12: Tail Start
- 13: Tail End
- 22: Withers
- 23: Throat

**Head & Face:**
- 14: Left Ear Base
- 15: Right Ear Base
- 16: Nose
- 17: Chin
- 18: Left Ear Tip
- 19: Right Ear Tip
- 20: Left Eye
- 21: Right Eye

**Note:** Only visible keypoints (visibility > 0) are displayed as red dots with white borders and numbered labels.
