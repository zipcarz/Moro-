Moro-
=====

...	...	@@ -1,8 +1,7 @@
1	1	 <?xml version="1.0" encoding="UTF-8" standalone="no"?>
2		-<document type="com.apple.InterfaceBuilder3.CocoaTouch.Storyboard.XIB" version="2.0" toolsVersion="5056" systemVersion="13D65" targetRuntime="iOS.CocoaTouch" variant="6xAndEarlier" propertyAccessControl="none" useAutolayout="YES" initialViewController="2">
2	+<document type="com.apple.InterfaceBuilder3.CocoaTouch.Storyboard.XIB" version="3.0" toolsVersion="5056" systemVersion="13D65" targetRuntime="iOS.CocoaTouch" propertyAccessControl="none" useAutolayout="YES" initialViewController="2">
3	3	     <dependencies>
4		-        <deployment defaultVersion="1536" identifier="iOS"/>
5		-        <development version="4600" identifier="xcode"/>
4	+        <deployment version="1552" defaultVersion="1536" identifier="iOS"/>
6	5	         <plugIn identifier="com.apple.InterfaceBuilder.IBCocoaTouchPlugin" version="3733"/>
7	6	     </dependencies>
8	7	     <scenes>
...	...	@@ -10,554 +9,328 @@
10	9	         <scene sceneID="5">
11	10	             <objects>
12	11	                 <viewController id="2" customClass="ViewController" sceneMemberID="viewController">
13		-                    <view key="view" contentMode="scaleToFill" id="3">
14		-                        <rect key="frame" x="0.0" y="20" width="320" height="548"/>
15		-                        <autoresizingMask key="autoresizingMask" flexibleMaxX="YES" flexibleMaxY="YES"/>
12	+                    <layoutGuides>
13	+                        <viewControllerLayoutGuide type="top" id="l3o-gc-LKh"/>
14	+                        <viewControllerLayoutGuide type="bottom" id="BWI-Tu-T44"/>
15	+                    </layoutGuides>
16	+                    <view key="view" contentMode="scaleToFill" id="SHD-Qg-HHW">
17	+                        <rect key="frame" x="0.0" y="0.0" width="320" height="480"/>
18	+                        <autoresizingMask key="autoresizingMask" widthSizable="YES" heightSizable="YES"/>
16	19	                         <subviews>
17		-                            <button opaque="NO" contentMode="scaleToFill" contentHorizontalAlignment="center" contentVerticalAlignment="center" buttonType="roundedRect" lineBreakMode="middleTruncation" translatesAutoresizingMaskIntoConstraints="NO" id="u1c-dm-6ud">
18		-                                <rect key="frame" x="27" y="99" width="75" height="23"/>
19		-                                <constraints>
20		-                                    <constraint firstAttribute="width" constant="75" id="gzp-Ht-e9u"/>
21		-                                    <constraint firstAttribute="height" constant="22" id="qMw-ci-3LE"/>
22		-                                </constraints>
23		-                                <fontDescription key="fontDescription" type="boldSystem" pointSize="15"/>
24		-                                <state key="normal" title="Wipe">
25		-                                    <color key="titleColor" red="0.19607843137254902" green="0.30980392156862746" blue="0.52156862745098043" alpha="1" colorSpace="calibratedRGB"/>
26		-                                    <color key="titleShadowColor" white="0.5" alpha="1" colorSpace="calibratedWhite"/>
27		-                                </state>
28		-                                <state key="highlighted">
29		-                                    <color key="titleColor" white="1" alpha="1" colorSpace="calibratedWhite"/>
30		-                                </state>
31		-                                <connections>
32		-                                    <action selector="StrWipe:" destination="2" eventType="touchUpInside" id="elv-gG-b8Y"/>
33		-                                </connections>
34		-                            </button>
35		-                            <button opaque="NO" contentMode="scaleToFill" contentHorizontalAlignment="center" contentVerticalAlignment="center" buttonType="roundedRect" lineBreakMode="middleTruncation" translatesAutoresizingMaskIntoConstraints="NO" id="Jv9-P4-E8a">
36		-                                <rect key="frame" x="135" y="97" width="73" height="23"/>
37		-                                <constraints>
38		-                                    <constraint firstAttribute="height" constant="22" id="9r7-ue-Fea"/>
39		-                                </constraints>
40		-                                <fontDescription key="fontDescription" type="boldSystem" pointSize="15"/>
41		-                                <state key="normal" title="Lock">
42		-                                    <color key="titleColor" red="0.19607843137254902" green="0.30980392156862746" blue="0.52156862745098043" alpha="1" colorSpace="calibratedRGB"/>
43		-                                    <color key="titleShadowColor" white="0.5" alpha="1" colorSpace="calibratedWhite"/>
44		-                                </state>
45		-                                <state key="highlighted">
46		-                                    <color key="titleColor" white="1" alpha="1" colorSpace="calibratedWhite"/>
47		-                                </state>
48		-                                <connections>
49		-                                    <action selector="StrLock:" destination="2" eventType="touchUpInside" id="OgH-Zx-aMn"/>
50		-                                </connections>
51		-                            </button>
52		-                            <button opaque="NO" contentMode="scaleToFill" contentHorizontalAlignment="center" contentVerticalAlignment="center" buttonType="roundedRect" lineBreakMode="middleTruncation" translatesAutoresizingMaskIntoConstraints="NO" id="YBo-gW-lDk">
53		-                                <rect key="frame" x="135" y="129" width="73" height="21"/>
54		-                                <fontDescription key="fontDescription" type="boldSystem" pointSize="15"/>
55		-                                <state key="normal" title="Unlock">
56		-                                    <color key="titleColor" red="0.19607843137254902" green="0.30980392156862746" blue="0.52156862745098043" alpha="1" colorSpace="calibratedRGB"/>
57		-                                    <color key="titleShadowColor" white="0.5" alpha="1" colorSpace="calibratedWhite"/>
58		-                                </state>
59		-                                <state key="highlighted">
60		-                                    <color key="titleColor" white="1" alpha="1" colorSpace="calibratedWhite"/>
61		-                                </state>
62		-                                <connections>
63		-                                    <action selector="StrUnlock:" destination="2" eventType="touchUpInside" id="V6Z-aj-QCJ"/>
64		-                                </connections>
65		-                            </button>
66		-                            <button opaque="NO" contentMode="scaleToFill" contentHorizontalAlignment="center" contentVerticalAlignment="center" buttonType="roundedRect" lineBreakMode="middleTruncation" translatesAutoresizingMaskIntoConstraints="NO" id="y86-FI-t8w">
67		-                                <rect key="frame" x="55" y="129" width="75" height="21"/>
68		-                                <constraints>
69		-                                    <constraint firstAttribute="width" constant="75" id="UNL-bY-1EJ"/>
70		-                                    <constraint firstAttribute="height" constant="20" id="bY3-Xj-vch"/>
71		-                                </constraints>
72		-                                <fontDescription key="fontDescription" type="boldSystem" pointSize="15"/>
73		-                                <state key="normal" title="Track">
74		-                                    <color key="titleColor" red="0.19607843137254902" green="0.30980392156862746" blue="0.52156862745098043" alpha="1" colorSpace="calibratedRGB"/>
75		-                                    <color key="titleShadowColor" white="0.5" alpha="1" colorSpace="calibratedWhite"/>
76		-                                </state>
77		-                                <state key="highlighted">
78		-                                    <color key="titleColor" white="1" alpha="1" colorSpace="calibratedWhite"/>
79		-                                </state>
80		-                                <connections>
81		-                                    <action selector="StringTrack:" destination="2" eventType="touchUpInside" id="USN-jH-sHZ"/>
82		-                                </connections>
83		-                            </button>
84		-                            <label opaque="NO" clipsSubviews="YES" userInteractionEnabled="NO" contentMode="left" text="NSString" lineBreakMode="tailTruncation" baselineAdjustment="alignBaselines" adjustsFontSizeToFit="NO" translatesAutoresizingMaskIntoConstraints="NO" id="XEw-Hc-TyQ">
85		-                                <rect key="frame" x="216" y="104" width="85" height="45"/>
86		-                                <constraints>
87		-                                    <constraint firstAttribute="height" constant="45" id="mBv-Xf-EK2"/>
88		-                                </constraints>
89		-                                <fontDescription key="fontDescription" type="system" pointSize="17"/>
90		-                                <color key="textColor" cocoaTouchSystemColor="darkTextColor"/>
91		-                                <nil key="highlightedColor"/>
92		-                            </label>
93		-                            <label opaque="NO" clipsSubviews="YES" userInteractionEnabled="NO" contentMode="left" text="?" lineBreakMode="tailTruncation" baselineAdjustment="alignBaselines" adjustsFontSizeToFit="NO" translatesAutoresizingMaskIntoConstraints="NO" id="Kjl-mI-E8q">
94		-                                <rect key="frame" x="20" y="157" width="300" height="22"/>
95		-                                <constraints>
96		-                                    <constraint firstAttribute="height" constant="22" id="8xG-hr-PsS"/>
97		-                                </constraints>
98		-                                <fontDescription key="fontDescription" type="system" pointSize="17"/>
99		-                                <color key="textColor" cocoaTouchSystemColor="darkTextColor"/>
100		-                                <nil key="highlightedColor"/>
101		-                            </label>
102		-                            <label opaque="NO" clipsSubviews="YES" userInteractionEnabled="NO" contentMode="left" text="?" lineBreakMode="wordWrap" numberOfLines="3" baselineAdjustment="alignBaselines" adjustsLetterSpacingToFitWidth="YES" adjustsFontSizeToFit="NO" preferredMaxLayoutWidth="300" translatesAutoresizingMaskIntoConstraints="NO" id="2oS-th-M8i">
103		-                                <rect key="frame" x="10" y="178" width="300" height="51"/>
104		-                                <constraints>
105		-                                    <constraint firstAttribute="height" constant="51" id="k08-t4-Nhm"/>
106		-                                    <constraint firstAttribute="width" constant="300" id="yQ1-O7-Wpf"/>
107		-                                </constraints>
108		-                                <fontDescription key="fontDescription" type="system" pointSize="12"/>
109		-                                <color key="textColor" cocoaTouchSystemColor="darkTextColor"/>
110		-                                <nil key="highlightedColor"/>
111		-                            </label>
112		-                            <toolbar opaque="NO" clearsContextBeforeDrawing="NO" contentMode="scaleToFill" translatesAutoresizingMaskIntoConstraints="NO" id="37q-JP-ijS">
113		-                                <rect key="frame" x="0.0" y="504" width="320" height="44"/>
20	+                            <toolbar opaque="NO" clearsContextBeforeDrawing="NO" contentMode="scaleToFill" fixedFrame="YES" translatesAutoresizingMaskIntoConstraints="NO" id="tN3-h2-AyF">
21	+                                <rect key="frame" x="-10" y="21" width="330" height="44"/>
22	+                                <autoresizingMask key="autoresizingMask" widthSizable="YES" flexibleMinY="YES"/>
114	23	                                 <items>
115		-                                    <barButtonItem title="Wipe" id="8ro-DT-jyq">
24	+                                    <barButtonItem title="wipeall" id="Gke-1y-h33">
116	25	                                         <connections>
117		-                                            <action selector="WipeAll:" destination="2" id="cwS-2y-W9F"/>
26	+                                            <action selector="WipeAll:" destination="2" id="LGk-r9-KYo"/>
118	27	                                         </connections>
119	28	                                     </barButtonItem>
120		-                                    <barButtonItem title="Lock" id="cXL-z9-589">
29	+                                    <barButtonItem title="lock" id="XAV-Wf-dGa">
121	30	                                         <connections>
122		-                                            <action selector="LockAll:" destination="2" id="hqN-cW-bra"/>
31	+                                            <action selector="LockAll:" destination="2" id="ZiC-rV-rF0"/>
123	32	                                         </connections>
124	33	                                     </barButtonItem>
125		-                                    <barButtonItem title="Unlock" id="W61-3Y-Z8u">
34	+                                    <barButtonItem title="unlock" id="dBx-aC-9AP">
126	35	                                         <connections>
127		-                                            <action selector="UnlockAll:" destination="2" id="8Pq-7K-c9N"/>
36	+                                            <action selector="UnlockAll:" destination="2" id="RpN-w6-fzc"/>
128	37	                                         </connections>
129	38	                                     </barButtonItem>
130		-                                    <barButtonItem title="Checksum" id="iWl-Kk-sxY">
39	+                                    <barButtonItem title="chksum" id="SkV-jG-22p">
131	40	                                         <connections>
132		-                                            <action selector="ChecksumAll:" destination="2" id="lnH-S3-o4b"/>
41	+                                            <action selector="ChecksumAll:" destination="2" id="5eu-6U-JON"/>
42	+                                        </connections>
43	+                                    </barButtonItem>
44	+                                    <barButtonItem title="prepexit" id="b03-L3-ykn">
45	+                                        <connections>
46	+                                            <action selector="SecureExit:" destination="2" id="iOo-QS-2N2"/>
133	47	                                         </connections>
134	48	                                     </barButtonItem>
135	49	                                 </items>
136	50	                             </toolbar>
137		-                            <label opaque="NO" clipsSubviews="YES" userInteractionEnabled="NO" contentMode="left" text="Label" lineBreakMode="tailTruncation" baselineAdjustment="alignBaselines" adjustsFontSizeToFit="NO" translatesAutoresizingMaskIntoConstraints="NO" id="Gu9-eK-rVY">
138		-                                <rect key="frame" x="0.0" y="228" width="320" height="1"/>
139		-                                <color key="backgroundColor" cocoaTouchSystemColor="darkTextColor"/>
140		-                                <constraints>
141		-                                    <constraint firstAttribute="height" constant="1" id="l5M-vT-LfK"/>
142		-                                </constraints>
143		-                                <fontDescription key="fontDescription" type="system" pointSize="17"/>
144		-                                <color key="textColor" cocoaTouchSystemColor="darkTextColor"/>
145		-                                <nil key="highlightedColor"/>
146		-                            </label>
147		-                            <button opaque="NO" contentMode="scaleToFill" contentHorizontalAlignment="center" contentVerticalAlignment="center" buttonType="roundedRect" lineBreakMode="middleTruncation" translatesAutoresizingMaskIntoConstraints="NO" id="dpm-HB-IJT">
148		-                                <rect key="frame" x="27" y="237" width="75" height="23"/>
149		-                                <constraints>
150		-                                    <constraint firstAttribute="height" constant="22" id="5Cc-pB-lgt"/>
151		-                                </constraints>
152		-                                <fontDescription key="fontDescription" type="boldSystem" pointSize="15"/>
153		-                                <state key="normal" title="Wipe">
154		-                                    <color key="titleColor" red="0.19607843137254902" green="0.30980392156862746" blue="0.52156862745098043" alpha="1" colorSpace="calibratedRGB"/>
155		-                                    <color key="titleShadowColor" white="0.5" alpha="1" colorSpace="calibratedWhite"/>
156		-                                </state>
157		-                                <state key="highlighted">
158		-                                    <color key="titleColor" white="1" alpha="1" colorSpace="calibratedWhite"/>
159		-                                </state>
160		-                                <connections>
161		-                                    <action selector="DataWipe:" destination="2" eventType="touchUpInside" id="Yy5-d2-DTh"/>
162		-                                </connections>
163		-                            </button>
164		-                            <button opaque="NO" contentMode="scaleToFill" contentHorizontalAlignment="center" contentVerticalAlignment="center" buttonType="roundedRect" lineBreakMode="middleTruncation" translatesAutoresizingMaskIntoConstraints="NO" id="Wdl-BB-pz1">
165		-                                <rect key="frame" x="124" y="237" width="73" height="23"/>
166		-                                <fontDescription key="fontDescription" type="boldSystem" pointSize="15"/>
167		-                                <state key="normal" title="Lock">
168		-                                    <color key="titleColor" red="0.19607843137254902" green="0.30980392156862746" blue="0.52156862745098043" alpha="1" colorSpace="calibratedRGB"/>
169		-                                    <color key="titleShadowColor" white="0.5" alpha="1" colorSpace="calibratedWhite"/>
170		-                                </state>
171		-                                <state key="highlighted">
172		-                                    <color key="titleColor" white="1" alpha="1" colorSpace="calibratedWhite"/>
173		-                                </state>
174		-                                <connections>
175		-                                    <action selector="DataLock:" destination="2" eventType="touchUpInside" id="2Q5-rH-Mbs"/>
176		-                                </connections>
177		-                            </button>
178		-                            <button opaque="NO" contentMode="scaleToFill" contentHorizontalAlignment="center" contentVerticalAlignment="center" buttonType="roundedRect" lineBreakMode="middleTruncation" translatesAutoresizingMaskIntoConstraints="NO" id="6tP-Vr-jxY">
179		-                                <rect key="frame" x="124" y="262" width="73" height="21"/>
180		-                                <constraints>
181		-                                    <constraint firstAttribute="height" constant="20" id="vJN-wd-qgB"/>
182		-                                </constraints>
183		-                                <fontDescription key="fontDescription" type="boldSystem" pointSize="15"/>
184		-                                <state key="normal" title="Unlock">
185		-                                    <color key="titleColor" red="0.19607843137254902" green="0.30980392156862746" blue="0.52156862745098043" alpha="1" colorSpace="calibratedRGB"/>
186		-                                    <color key="titleShadowColor" white="0.5" alpha="1" colorSpace="calibratedWhite"/>
187		-                                </state>
188		-                                <state key="highlighted">
189		-                                    <color key="titleColor" white="1" alpha="1" colorSpace="calibratedWhite"/>
190		-                                </state>
191		-                                <connections>
192		-                                    <action selector="DataUnlock:" destination="2" eventType="touchUpInside" id="UFX-nC-44H"/>
193		-                                </connections>
194		-                            </button>
195		-                            <button opaque="NO" contentMode="scaleToFill" contentHorizontalAlignment="center" contentVerticalAlignment="center" buttonType="roundedRect" lineBreakMode="middleTruncation" translatesAutoresizingMaskIntoConstraints="NO" id="G5L-hc-uEX">
196		-                                <rect key="frame" x="27" y="264" width="75" height="21"/>
197		-                                <constraints>
198		-                                    <constraint firstAttribute="height" constant="20" id="uhE-wH-C5r"/>
199		-                                </constraints>
200		-                                <fontDescription key="fontDescription" type="boldSystem" pointSize="15"/>
201		-                                <state key="normal" title="Track">
202		-                                    <color key="titleColor" red="0.19607843137254902" green="0.30980392156862746" blue="0.52156862745098043" alpha="1" colorSpace="calibratedRGB"/>
203		-                                    <color key="titleShadowColor" white="0.5" alpha="1" colorSpace="calibratedWhite"/>
204		-                                </state>
205		-                                <state key="highlighted">
206		-                                    <color key="titleColor" white="1" alpha="1" colorSpace="calibratedWhite"/>
207		-                                </state>
208		-                                <connections>
209		-                                    <action selector="DataTrack:" destination="2" eventType="touchUpInside" id="06o-b5-IPn"/>
210		-                                </connections>
211		-                            </button>
212		-                            <label opaque="NO" clipsSubviews="YES" userInteractionEnabled="NO" contentMode="left" text="NSData" lineBreakMode="tailTruncation" baselineAdjustment="alignBaselines" adjustsFontSizeToFit="NO" translatesAutoresizingMaskIntoConstraints="NO" id="GmH-vb-QuB">
213		-                                <rect key="frame" x="216" y="237" width="85" height="45"/>
214		-                                <constraints>
215		-                                    <constraint firstAttribute="height" constant="45" id="UQS-eR-n29"/>
216		-                                    <constraint firstAttribute="width" constant="85" id="wea-Rc-cvz"/>
217		-                                </constraints>
218		-                                <fontDescription key="fontDescription" type="system" pointSize="17"/>
219		-                                <color key="textColor" cocoaTouchSystemColor="darkTextColor"/>
220		-                                <nil key="highlightedColor"/>
221		-                            </label>
222		-                            <label opaque="NO" clipsSubviews="YES" userInteractionEnabled="NO" contentMode="left" text="?" lineBreakMode="tailTruncation" baselineAdjustment="alignBaselines" adjustsFontSizeToFit="NO" translatesAutoresizingMaskIntoConstraints="NO" id="xLN-TM-gKU">
223		-                                <rect key="frame" x="20" y="292" width="300" height="22"/>
224		-                                <constraints>
225		-                                    <constraint firstAttribute="height" constant="22" id="4ex-1j-X2S"/>
226		-                                </constraints>
227		-                                <fontDescription key="fontDescription" type="system" pointSize="17"/>
228		-                                <color key="textColor" cocoaTouchSystemColor="darkTextColor"/>
229		-                                <nil key="highlightedColor"/>
230		-                            </label>
231		-                            <label opaque="NO" clipsSubviews="YES" userInteractionEnabled="NO" contentMode="left" text="?" lineBreakMode="wordWrap" numberOfLines="3" baselineAdjustment="alignBaselines" adjustsLetterSpacingToFitWidth="YES" adjustsFontSizeToFit="NO" preferredMaxLayoutWidth="300" translatesAutoresizingMaskIntoConstraints="NO" id="qYb-w8-oEj">
232		-                                <rect key="frame" x="20" y="315" width="300" height="51"/>
233		-                                <constraints>
234		-                                    <constraint firstAttribute="height" constant="51" id="QJh-GN-hCA"/>
235		-                                </constraints>
236		-                                <fontDescription key="fontDescription" type="system" pointSize="12"/>
237		-                                <color key="textColor" cocoaTouchSystemColor="darkTextColor"/>
238		-                                <nil key="highlightedColor"/>
239		-                            </label>
240		-                            <label opaque="NO" clipsSubviews="YES" userInteractionEnabled="NO" contentMode="left" text="Label" lineBreakMode="tailTruncation" baselineAdjustment="alignBaselines" adjustsFontSizeToFit="NO" translatesAutoresizingMaskIntoConstraints="NO" id="2H6-VV-Dvf">
241		-                                <rect key="frame" x="0.0" y="366" width="320" height="1"/>
242		-                                <color key="backgroundColor" cocoaTouchSystemColor="darkTextColor"/>
243		-                                <constraints>
244		-                                    <constraint firstAttribute="height" constant="1" id="8yd-xA-sj8"/>
245		-                                </constraints>
246		-                                <fontDescription key="fontDescription" type="system" pointSize="17"/>
247		-                                <color key="textColor" cocoaTouchSystemColor="darkTextColor"/>
248		-                                <nil key="highlightedColor"/>
249		-                            </label>
250		-                            <button opaque="NO" contentMode="scaleToFill" contentHorizontalAlignment="center" contentVerticalAlignment="center" buttonType="roundedRect" lineBreakMode="middleTruncation" translatesAutoresizingMaskIntoConstraints="NO" id="P7g-Ha-dBr">
251		-                                <rect key="frame" x="20" y="375" width="75" height="23"/>
252		-                                <constraints>
253		-                                    <constraint firstAttribute="width" constant="75" id="vPT-AS-gjC"/>
254		-                                    <constraint firstAttribute="height" constant="22" id="x6n-Hq-sGt"/>
255		-                                </constraints>
256		-                                <fontDescription key="fontDescription" type="boldSystem" pointSize="15"/>
257		-                                <state key="normal" title="Wipe">
258		-                                    <color key="titleColor" red="0.19607843137254902" green="0.30980392156862746" blue="0.52156862745098043" alpha="1" colorSpace="calibratedRGB"/>
259		-                                    <color key="titleShadowColor" white="0.5" alpha="1" colorSpace="calibratedWhite"/>
260		-                                </state>
261		-                                <state key="highlighted">
262		-                                    <color key="titleColor" white="1" alpha="1" colorSpace="calibratedWhite"/>
263		-                                </state>
264		-                                <connections>
265		-                                    <action selector="NumberWipe:" destination="2" eventType="touchUpInside" id="5Dy-XK-FkL"/>
266		-                                </connections>
267		-                            </button>
268		-                            <button opaque="NO" contentMode="scaleToFill" contentHorizontalAlignment="center" contentVerticalAlignment="center" buttonType="roundedRect" lineBreakMode="middleTruncation" translatesAutoresizingMaskIntoConstraints="NO" id="ETE-vt-zWY">
269		-                                <rect key="frame" x="100" y="375" width="73" height="23"/>
270		-                                <fontDescription key="fontDescription" type="boldSystem" pointSize="15"/>
271		-                                <state key="normal" title="Lock">
272		-                                    <color key="titleColor" red="0.19607843137254902" green="0.30980392156862746" blue="0.52156862745098043" alpha="1" colorSpace="calibratedRGB"/>
273		-                                    <color key="titleShadowColor" white="0.5" alpha="1" colorSpace="calibratedWhite"/>
274		-                                </state>
275		-                                <state key="highlighted">
276		-                                    <color key="titleColor" white="1" alpha="1" colorSpace="calibratedWhite"/>
277		-                                </state>
278		-                                <connections>
279		-                                    <action selector="NumberLock:" destination="2" eventType="touchUpInside" id="AGp-FO-Beq"/>
280		-                                </connections>
281		-                            </button>
282		-                            <button opaque="NO" contentMode="scaleToFill" contentHorizontalAlignment="center" contentVerticalAlignment="center" buttonType="roundedRect" lineBreakMode="middleTruncation" translatesAutoresizingMaskIntoConstraints="NO" id="yPn-Yt-de3">
283		-                                <rect key="frame" x="100" y="400" width="73" height="21"/>
284		-                                <fontDescription key="fontDescription" type="boldSystem" pointSize="15"/>
285		-                                <state key="normal" title="Unlock">
286		-                                    <color key="titleColor" red="0.19607843137254902" green="0.30980392156862746" blue="0.52156862745098043" alpha="1" colorSpace="calibratedRGB"/>
287		-                                    <color key="titleShadowColor" white="0.5" alpha="1" colorSpace="calibratedWhite"/>
288		-                                </state>
289		-                                <state key="highlighted">
290		-                                    <color key="titleColor" white="1" alpha="1" colorSpace="calibratedWhite"/>
291		-                                </state>
292		-                                <connections>
293		-                                    <action selector="NumberUnlock:" destination="2" eventType="touchUpInside" id="Jlc-un-wHa"/>
294		-                                </connections>
295		-                            </button>
296		-                            <button opaque="NO" contentMode="scaleToFill" contentHorizontalAlignment="center" contentVerticalAlignment="center" buttonType="roundedRect" lineBreakMode="middleTruncation" translatesAutoresizingMaskIntoConstraints="NO" id="47A-8u-V1R">
297		-                                <rect key="frame" x="20" y="400" width="75" height="21"/>
298		-                                <constraints>
299		-                                    <constraint firstAttribute="height" constant="20" id="EjV-86-wNf"/>
300		-                                </constraints>
301		-                                <fontDescription key="fontDescription" type="boldSystem" pointSize="15"/>
302		-                                <state key="normal" title="Track">
303		-                                    <color key="titleColor" red="0.19607843137254902" green="0.30980392156862746" blue="0.52156862745098043" alpha="1" colorSpace="calibratedRGB"/>
304		-                                    <color key="titleShadowColor" white="0.5" alpha="1" colorSpace="calibratedWhite"/>
305		-                                </state>
306		-                                <state key="highlighted">
307		-                                    <color key="titleColor" white="1" alpha="1" colorSpace="calibratedWhite"/>
308		-                                </state>
309		-                                <connections>
310		-                                    <action selector="NumberTrack:" destination="2" eventType="touchUpInside" id="N2b-Wa-c7c"/>
311		-                                </connections>
312		-                            </button>
313		-                            <label opaque="NO" clipsSubviews="YES" userInteractionEnabled="NO" contentMode="left" text="NSNumber" lineBreakMode="tailTruncation" baselineAdjustment="alignBaselines" adjustsFontSizeToFit="NO" translatesAutoresizingMaskIntoConstraints="NO" id="d0F-qV-STH">
314		-                                <rect key="frame" x="181" y="374" width="85" height="45"/>
315		-                                <constraints>
316		-                                    <constraint firstAttribute="height" constant="45" id="wuG-1h-N0D"/>
317		-                                </constraints>
318		-                                <fontDescription key="fontDescription" type="system" pointSize="17"/>
319		-                                <color key="textColor" cocoaTouchSystemColor="darkTextColor"/>
320		-                                <nil key="highlightedColor"/>
321		-                            </label>
322		-                            <label opaque="NO" clipsSubviews="YES" userInteractionEnabled="NO" contentMode="left" text="?" lineBreakMode="tailTruncation" baselineAdjustment="alignBaselines" adjustsFontSizeToFit="NO" translatesAutoresizingMaskIntoConstraints="NO" id="lvZ-lv-UPk">
323		-                                <rect key="frame" x="20" y="427" width="300" height="22"/>
324		-                                <constraints>
325		-                                    <constraint firstAttribute="height" constant="22" id="q5H-b6-Obu"/>
326		-                                </constraints>
327		-                                <fontDescription key="fontDescription" type="system" pointSize="17"/>
328		-                                <color key="textColor" cocoaTouchSystemColor="darkTextColor"/>
329		-                                <nil key="highlightedColor"/>
330		-                            </label>
331		-                            <label opaque="NO" clipsSubviews="YES" userInteractionEnabled="NO" contentMode="left" text="?" lineBreakMode="wordWrap" numberOfLines="3" baselineAdjustment="alignBaselines" adjustsLetterSpacingToFitWidth="YES" adjustsFontSizeToFit="NO" preferredMaxLayoutWidth="300" translatesAutoresizingMaskIntoConstraints="NO" id="lBU-4d-AnD">
332		-                                <rect key="frame" x="20" y="452" width="300" height="51"/>
333		-                                <constraints>
334		-                                    <constraint firstAttribute="height" constant="51" id="e9q-lr-RtI"/>
335		-                                </constraints>
336		-                                <fontDescription key="fontDescription" type="system" pointSize="12"/>
337		-                                <color key="textColor" cocoaTouchSystemColor="darkTextColor"/>
338		-                                <nil key="highlightedColor"/>
339		-                            </label>
340		-                            <label opaque="NO" clipsSubviews="YES" userInteractionEnabled="NO" contentMode="left" text="Label" lineBreakMode="tailTruncation" baselineAdjustment="alignBaselines" adjustsFontSizeToFit="NO" translatesAutoresizingMaskIntoConstraints="NO" id="r7R-D1-lVt">
341		-                                <rect key="frame" x="0.0" y="503" width="320" height="1"/>
342		-                                <color key="backgroundColor" cocoaTouchSystemColor="darkTextColor"/>
343		-                                <constraints>
344		-                                    <constraint firstAttribute="height" constant="1" id="fJV-fq-haI"/>
345		-                                </constraints>
346		-                                <fontDescription key="fontDescription" type="system" pointSize="17"/>
347		-                                <color key="textColor" cocoaTouchSystemColor="darkTextColor"/>
348		-                                <nil key="highlightedColor"/>
349		-                            </label>
350		-                            <button opaque="NO" contentMode="scaleToFill" contentHorizontalAlignment="center" contentVerticalAlignment="center" buttonType="roundedRect" lineBreakMode="middleTruncation" translatesAutoresizingMaskIntoConstraints="NO" id="lN4-ps-aIf">
351		-                                <rect key="frame" x="37" y="2" width="75" height="23"/>
352		-                                <constraints>
353		-                                    <constraint firstAttribute="height" constant="22" id="INl-SV-COw"/>
354		-                                    <constraint firstAttribute="width" constant="75" id="YfP-63-EBA"/>
355		-                                </constraints>
356		-                                <fontDescription key="fontDescription" type="boldSystem" pointSize="15"/>
357		-                                <state key="normal" title="Wipe">
358		-                                    <color key="titleColor" red="0.19607843137254902" green="0.30980392156862746" blue="0.52156862745098043" alpha="1" colorSpace="calibratedRGB"/>
359		-                                    <color key="titleShadowColor" white="0.5" alpha="1" colorSpace="calibratedWhite"/>
360		-                                </state>
361		-                                <state key="highlighted">
362		-                                    <color key="titleColor" white="1" alpha="1" colorSpace="calibratedWhite"/>
363		-                                </state>
364		-                                <connections>
365		-                                    <action selector="ArrayWipe:" destination="2" eventType="touchUpInside" id="C3s-ao-tQO"/>
366		-                                    <action selector="StrWipe:" destination="2" eventType="touchUpInside" id="w2O-vV-WVF"/>
367		-                                </connections>
368		-                            </button>
369		-                            <button opaque="NO" contentMode="scaleToFill" contentHorizontalAlignment="center" contentVerticalAlignment="center" buttonType="roundedRect" lineBreakMode="middleTruncation" translatesAutoresizingMaskIntoConstraints="NO" id="AEQ-bX-01b">
370		-                                <rect key="frame" x="140" y="2" width="73" height="23"/>
371		-                                <fontDescription key="fontDescription" type="boldSystem" pointSize="15"/>
372		-                                <state key="normal" title="Lock">
373		-                                    <color key="titleColor" red="0.19607843137254902" green="0.30980392156862746" blue="0.52156862745098043" alpha="1" colorSpace="calibratedRGB"/>
374		-                                    <color key="titleShadowColor" white="0.5" alpha="1" colorSpace="calibratedWhite"/>
375		-                                </state>
376		-                                <state key="highlighted">
377		-                                    <color key="titleColor" white="1" alpha="1" colorSpace="calibratedWhite"/>
378		-                                </state>
379		-                                <connections>
380		-                                    <action selector="ArrayLock:" destination="2" eventType="touchUpInside" id="uu2-Yy-JFf"/>
381		-                                    <action selector="StrLock:" destination="2" eventType="touchUpInside" id="xvd-gI-31n"/>
382		-                                </connections>
383		-                            </button>
384		-                            <button opaque="NO" contentMode="scaleToFill" contentHorizontalAlignment="center" contentVerticalAlignment="center" buttonType="roundedRect" lineBreakMode="middleTruncation" translatesAutoresizingMaskIntoConstraints="NO" id="uPq-tp-wen">
385		-                                <rect key="frame" x="140" y="32" width="73" height="21"/>
386		-                                <fontDescription key="fontDescription" type="boldSystem" pointSize="15"/>
387		-                                <state key="normal" title="Unlock">
388		-                                    <color key="titleColor" red="0.19607843137254902" green="0.30980392156862746" blue="0.52156862745098043" alpha="1" colorSpace="calibratedRGB"/>
389		-                                    <color key="titleShadowColor" white="0.5" alpha="1" colorSpace="calibratedWhite"/>
390		-                                </state>
391		-                                <state key="highlighted">
392		-                                    <color key="titleColor" white="1" alpha="1" colorSpace="calibratedWhite"/>
393		-                                </state>
394		-                                <connections>
395		-                                    <action selector="ArrayUnlock:" destination="2" eventType="touchUpInside" id="4xk-JO-dBq"/>
396		-                                    <action selector="StrUnlock:" destination="2" eventType="touchUpInside" id="1rL-5x-oQv"/>
397		-                                </connections>
398		-                            </button>
399		-                            <button opaque="NO" contentMode="scaleToFill" contentHorizontalAlignment="center" contentVerticalAlignment="center" buttonType="roundedRect" lineBreakMode="middleTruncation" translatesAutoresizingMaskIntoConstraints="NO" id="Atv-XN-z4x">
400		-                                <rect key="frame" x="37" y="32" width="75" height="21"/>
401		-                                <constraints>
402		-                                    <constraint firstAttribute="height" constant="20" id="ca9-yL-rxO"/>
403		-                                </constraints>
404		-                                <fontDescription key="fontDescription" type="boldSystem" pointSize="15"/>
405		-                                <state key="normal" title="Track">
406		-                                    <color key="titleColor" red="0.19607843137254902" green="0.30980392156862746" blue="0.52156862745098043" alpha="1" colorSpace="calibratedRGB"/>
407		-                                    <color key="titleShadowColor" white="0.5" alpha="1" colorSpace="calibratedWhite"/>
408		-                                </state>
409		-                                <state key="highlighted">
410		-                                    <color key="titleColor" white="1" alpha="1" colorSpace="calibratedWhite"/>
411		-                                </state>
412		-                                <connections>
413		-                                    <action selector="ArrayTrack:" destination="2" eventType="touchUpInside" id="ZrA-3G-XBu"/>
414		-                                </connections>
415		-                            </button>
416		-                            <label opaque="NO" clipsSubviews="YES" userInteractionEnabled="NO" contentMode="left" text="NSArray" lineBreakMode="tailTruncation" baselineAdjustment="alignBaselines" adjustsFontSizeToFit="NO" translatesAutoresizingMaskIntoConstraints="NO" id="dWj-7L-KOU">
417		-                                <rect key="frame" x="235" y="14" width="85" height="45"/>
418		-                                <constraints>
419		-                                    <constraint firstAttribute="height" constant="45" id="DLG-z9-tdR"/>
420		-                                    <constraint firstAttribute="width" constant="85" id="ZlI-DR-GE2"/>
421		-                                </constraints>
422		-                                <fontDescription key="fontDescription" type="system" pointSize="17"/>
423		-                                <color key="textColor" cocoaTouchSystemColor="darkTextColor"/>
424		-                                <nil key="highlightedColor"/>
425		-                            </label>
426		-                            <label opaque="NO" clipsSubviews="YES" userInteractionEnabled="NO" contentMode="left" text="?" lineBreakMode="tailTruncation" baselineAdjustment="alignBaselines" adjustsFontSizeToFit="NO" translatesAutoresizingMaskIntoConstraints="NO" id="haZ-1C-gLf">
427		-                                <rect key="frame" x="20" y="55" width="300" height="22"/>
428		-                                <constraints>
429		-                                    <constraint firstAttribute="height" constant="22" id="Dty-E8-UBX"/>
430		-                                </constraints>
431		-                                <fontDescription key="fontDescription" type="system" pointSize="17"/>
432		-                                <color key="textColor" cocoaTouchSystemColor="darkTextColor"/>
433		-                                <nil key="highlightedColor"/>
434		-                            </label>
435		-                            <label opaque="NO" clipsSubviews="YES" userInteractionEnabled="NO" contentMode="left" text="Label" lineBreakMode="tailTruncation" baselineAdjustment="alignBaselines" adjustsFontSizeToFit="NO" translatesAutoresizingMaskIntoConstraints="NO" id="FdT-JW-BaB">
436		-                                <rect key="frame" x="0.0" y="88" width="320" height="1"/>
437		-                                <color key="backgroundColor" cocoaTouchSystemColor="darkTextColor"/>
438		-                                <constraints>
439		-                                    <constraint firstAttribute="height" constant="1" id="NOC-VE-IZx"/>
440		-                                </constraints>
441		-                                <fontDescription key="fontDescription" type="system" pointSize="17"/>
442		-                                <color key="textColor" cocoaTouchSystemColor="darkTextColor"/>
443		-                                <nil key="highlightedColor"/>
444		-                            </label>
51	+                            <scrollView clipsSubviews="YES" multipleTouchEnabled="YES" contentMode="scaleToFill" fixedFrame="YES" translatesAutoresizingMaskIntoConstraints="NO" id="Ojf-xA-zUB">
52	+                                <rect key="frame" x="0.0" y="65" width="320" height="415"/>
53	+                                <autoresizingMask key="autoresizingMask" widthSizable="YES" heightSizable="YES"/>
54	+                                <subviews>
55	+                                    <label opaque="NO" clipsSubviews="YES" userInteractionEnabled="NO" contentMode="left" horizontalHuggingPriority="251" verticalHuggingPriority="251" fixedFrame="YES" text="NSString" lineBreakMode="tailTruncation" baselineAdjustment="alignBaselines" adjustsFontSizeToFit="NO" translatesAutoresizingMaskIntoConstraints="NO" id="Hnr-8q-edy">
56	+                                        <rect key="frame" x="16" y="12" width="69" height="21"/>
57	+                                        <autoresizingMask key="autoresizingMask" flexibleMaxX="YES" flexibleMaxY="YES"/>
58	+                                        <fontDescription key="fontDescription" type="system" pointSize="17"/>
59	+                                        <color key="textColor" cocoaTouchSystemColor="darkTextColor"/>
60	+                                        <nil key="highlightedColor"/>
61	+                                    </label>
62	+                                    <button opaque="NO" contentMode="scaleToFill" fixedFrame="YES" contentHorizontalAlignment="center" contentVerticalAlignment="center" buttonType="roundedRect" lineBreakMode="middleTruncation" translatesAutoresizingMaskIntoConstraints="NO" id="Jfi-hL-9qb">
63	+                                        <rect key="frame" x="109" y="8" width="33" height="30"/>
64	+                                        <autoresizingMask key="autoresizingMask" flexibleMaxX="YES" flexibleMaxY="YES"/>
65	+                                        <state key="normal" title="wipe">
66	+                                            <color key="titleShadowColor" white="0.5" alpha="1" colorSpace="calibratedWhite"/>
67	+                                        </state>
68	+                                        <connections>
69	+                                            <action selector="StrWipe:" destination="2" eventType="touchUpInside" id="9Tu-3w-Ewo"/>
70	+                                        </connections>
71	+                                    </button>
72	+                                    <button opaque="NO" contentMode="scaleToFill" fixedFrame="YES" contentHorizontalAlignment="center" contentVerticalAlignment="center" buttonType="roundedRect" lineBreakMode="middleTruncation" translatesAutoresizingMaskIntoConstraints="NO" id="CZ7-Nx-lZ1">
73	+                                        <rect key="frame" x="226" y="8" width="30" height="30"/>
74	+                                        <autoresizingMask key="autoresizingMask" flexibleMaxX="YES" flexibleMaxY="YES"/>
75	+                                        <state key="normal" title="lock">
76	+                                            <color key="titleShadowColor" white="0.5" alpha="1" colorSpace="calibratedWhite"/>
77	+                                        </state>
78	+                                        <connections>
79	+                                            <action selector="StrLock:" destination="2" eventType="touchUpInside" id="MgD-rs-XrQ"/>
80	+                                        </connections>
81	+                                    </button>
82	+                                    <button opaque="NO" contentMode="scaleToFill" fixedFrame="YES" contentHorizontalAlignment="center" contentVerticalAlignment="center" buttonType="roundedRect" lineBreakMode="middleTruncation" translatesAutoresizingMaskIntoConstraints="NO" id="gdT-F0-1nU">
83	+                                        <rect key="frame" x="267" y="8" width="46" height="30"/>
84	+                                        <autoresizingMask key="autoresizingMask" flexibleMaxX="YES" flexibleMaxY="YES"/>
85	+                                        <state key="normal" title="unlock">
86	+                                            <color key="titleShadowColor" white="0.5" alpha="1" colorSpace="calibratedWhite"/>
87	+                                        </state>
88	+                                        <connections>
89	+                                            <action selector="StrUnlock:" destination="2" eventType="touchUpInside" id="2Ip-27-rJC"/>
90	+                                        </connections>
91	+                                    </button>
92	+                                    <button opaque="NO" contentMode="scaleToFill" fixedFrame="YES" contentHorizontalAlignment="center" contentVerticalAlignment="center" buttonType="roundedRect" lineBreakMode="middleTruncation" translatesAutoresizingMaskIntoConstraints="NO" id="omn-rx-RLc">
93	+                                        <rect key="frame" x="149" y="8" width="61" height="30"/>
94	+                                        <autoresizingMask key="autoresizingMask" flexibleMaxX="YES" flexibleMaxY="YES"/>
95	+                                        <state key="normal" title="track">
96	+                                            <color key="titleShadowColor" white="0.5" alpha="1" colorSpace="calibratedWhite"/>
97	+                                        </state>
98	+                                        <connections>
99	+                                            <action selector="StringTrack:" destination="2" eventType="touchUpInside" id="cwf-10-FO1"/>
100	+                                        </connections>
101	+                                    </button>
102	+                                    <label opaque="NO" clipsSubviews="YES" userInteractionEnabled="NO" contentMode="left" horizontalHuggingPriority="251" verticalHuggingPriority="251" fixedFrame="YES" text="StrLabel" lineBreakMode="tailTruncation" baselineAdjustment="alignBaselines" adjustsFontSizeToFit="NO" translatesAutoresizingMaskIntoConstraints="NO" id="KRd-cw-0TM">
103	+                                        <rect key="frame" x="16" y="41" width="292" height="21"/>
104	+                                        <autoresizingMask key="autoresizingMask" flexibleMaxX="YES" flexibleMaxY="YES"/>
105	+                                        <fontDescription key="fontDescription" type="system" pointSize="17"/>
106	+                                        <nil key="highlightedColor"/>
107	+                                    </label>
108	+                                    <label opaque="NO" clipsSubviews="YES" userInteractionEnabled="NO" contentMode="left" horizontalHuggingPriority="251" verticalHuggingPriority="251" fixedFrame="YES" text="StrHex" lineBreakMode="tailTruncation" numberOfLines="3" baselineAdjustment="alignBaselines" adjustsFontSizeToFit="NO" preferredMaxLayoutWidth="292" translatesAutoresizingMaskIntoConstraints="NO" id="ZfG-il-4O9">
109	+                                        <rect key="frame" x="16" y="70" width="292" height="42"/>
110	+                                        <autoresizingMask key="autoresizingMask" flexibleMaxX="YES" flexibleMaxY="YES"/>
111	+                                        <fontDescription key="fontDescription" name="Courier" family="Courier" pointSize="12"/>
112	+                                        <nil key="highlightedColor"/>
113	+                                    </label>
114	+                                    <label opaque="NO" clipsSubviews="YES" userInteractionEnabled="NO" contentMode="left" horizontalHuggingPriority="251" verticalHuggingPriority="251" fixedFrame="YES" text="                                                                   " lineBreakMode="tailTruncation" baselineAdjustment="alignBaselines" adjustsFontSizeToFit="NO" translatesAutoresizingMaskIntoConstraints="NO" id="0VH-QF-3rL">
115	+                                        <rect key="frame" x="0.0" y="120" width="322" height="5"/>
116	+                                        <autoresizingMask key="autoresizingMask" flexibleMaxX="YES" flexibleMaxY="YES"/>
117	+                                        <color key="backgroundColor" white="0.0" alpha="1" colorSpace="calibratedWhite"/>
118	+                                        <fontDescription key="fontDescription" type="system" pointSize="17"/>
119	+                                        <nil key="highlightedColor"/>
120	+                                    </label>
121	+                                    <label opaque="NO" clipsSubviews="YES" userInteractionEnabled="NO" contentMode="left" horizontalHuggingPriority="251" verticalHuggingPriority="251" fixedFrame="YES" text="NSData" lineBreakMode="tailTruncation" baselineAdjustment="alignBaselines" adjustsFontSizeToFit="NO" translatesAutoresizingMaskIntoConstraints="NO" id="H7x-B4-en9">
122	+                                        <rect key="frame" x="16" y="137" width="60" height="21"/>
123	+                                        <autoresizingMask key="autoresizingMask" flexibleMaxX="YES" flexibleMaxY="YES"/>
124	+                                        <fontDescription key="fontDescription" type="system" pointSize="17"/>
125	+                                        <color key="textColor" cocoaTouchSystemColor="darkTextColor"/>
126	+                                        <nil key="highlightedColor"/>
127	+                                    </label>
128	+                                    <button opaque="NO" contentMode="scaleToFill" fixedFrame="YES" contentHorizontalAlignment="center" contentVerticalAlignment="center" buttonType="roundedRect" lineBreakMode="middleTruncation" translatesAutoresizingMaskIntoConstraints="NO" id="Tmf-rb-gZj">
129	+                                        <rect key="frame" x="109" y="133" width="33" height="30"/>
130	+                                        <autoresizingMask key="autoresizingMask" flexibleMaxX="YES" flexibleMaxY="YES"/>
131	+                                        <state key="normal" title="wipe">
132	+                                            <color key="titleShadowColor" white="0.5" alpha="1" colorSpace="calibratedWhite"/>
133	+                                        </state>
134	+                                        <connections>
135	+                                            <action selector="DataWipe:" destination="2" eventType="touchUpInside" id="sIq-28-oay"/>
136	+                                        </connections>
137	+                                    </button>
138	+                                    <button opaque="NO" contentMode="scaleToFill" fixedFrame="YES" contentHorizontalAlignment="center" contentVerticalAlignment="center" buttonType="roundedRect" lineBreakMode="middleTruncation" translatesAutoresizingMaskIntoConstraints="NO" id="Nws-Ik-xsc">
139	+                                        <rect key="frame" x="226" y="133" width="30" height="30"/>
140	+                                        <autoresizingMask key="autoresizingMask" flexibleMaxX="YES" flexibleMaxY="YES"/>
141	+                                        <state key="normal" title="lock">
142	+                                            <color key="titleShadowColor" white="0.5" alpha="1" colorSpace="calibratedWhite"/>
143	+                                        </state>
144	+                                        <connections>
145	+                                            <action selector="DataLock:" destination="2" eventType="touchUpInside" id="YWf-3N-DX0"/>
146	+                                        </connections>
147	+                                    </button>
148	+                                    <button opaque="NO" contentMode="scaleToFill" fixedFrame="YES" contentHorizontalAlignment="center" contentVerticalAlignment="center" buttonType="roundedRect" lineBreakMode="middleTruncation" translatesAutoresizingMaskIntoConstraints="NO" id="tTy-hU-zEX">
149	+                                        <rect key="frame" x="267" y="133" width="46" height="30"/>
150	+                                        <autoresizingMask key="autoresizingMask" flexibleMaxX="YES" flexibleMaxY="YES"/>
151	+                                        <state key="normal" title="unlock">
152	+                                            <color key="titleShadowColor" white="0.5" alpha="1" colorSpace="calibratedWhite"/>
153	+                                        </state>
154	+                                        <connections>
155	+                                            <action selector="DataUnlock:" destination="2" eventType="touchUpInside" id="NhB-cD-7CO"/>
156	+                                        </connections>
157	+                                    </button>
158	+                                    <button opaque="NO" contentMode="scaleToFill" fixedFrame="YES" contentHorizontalAlignment="center" contentVerticalAlignment="center" buttonType="roundedRect" lineBreakMode="middleTruncation" translatesAutoresizingMaskIntoConstraints="NO" id="Qtb-hp-9kW">
159	+                                        <rect key="frame" x="149" y="133" width="61" height="30"/>
160	+                                        <autoresizingMask key="autoresizingMask" flexibleMaxX="YES" flexibleMaxY="YES"/>
161	+                                        <state key="normal" title="track">
162	+                                            <color key="titleShadowColor" white="0.5" alpha="1" colorSpace="calibratedWhite"/>
163	+                                        </state>
164	+                                        <connections>
165	+                                            <action selector="DataTrack:" destination="2" eventType="touchUpInside" id="JBZ-38-DE2"/>
166	+                                        </connections>
167	+                                    </button>
168	+                                    <label opaque="NO" clipsSubviews="YES" userInteractionEnabled="NO" contentMode="left" horizontalHuggingPriority="251" verticalHuggingPriority="251" fixedFrame="YES" text="DataLabel" lineBreakMode="tailTruncation" baselineAdjustment="alignBaselines" adjustsFontSizeToFit="NO" translatesAutoresizingMaskIntoConstraints="NO" id="B1u-7b-1Aq">
169	+                                        <rect key="frame" x="16" y="166" width="292" height="21"/>
170	+                                        <autoresizingMask key="autoresizingMask" flexibleMaxX="YES" flexibleMaxY="YES"/>
171	+                                        <fontDescription key="fontDescription" type="system" pointSize="17"/>
172	+                                        <nil key="highlightedColor"/>
173	+                                    </label>
174	+                                    <label opaque="NO" clipsSubviews="YES" userInteractionEnabled="NO" contentMode="left" horizontalHuggingPriority="251" verticalHuggingPriority="251" fixedFrame="YES" text="DataHex" lineBreakMode="tailTruncation" baselineAdjustment="alignBaselines" adjustsFontSizeToFit="NO" translatesAutoresizingMaskIntoConstraints="NO" id="xRQ-ZY-YJl">
175	+                                        <rect key="frame" x="16" y="195" width="292" height="21"/>
176	+                                        <autoresizingMask key="autoresizingMask" flexibleMaxX="YES" flexibleMaxY="YES"/>
177	+                                        <fontDescription key="fontDescription" name="Courier" family="Courier" pointSize="12"/>
178	+                                        <nil key="highlightedColor"/>
179	+                                    </label>
180	+                                    <label opaque="NO" clipsSubviews="YES" userInteractionEnabled="NO" contentMode="left" horizontalHuggingPriority="251" verticalHuggingPriority="251" fixedFrame="YES" text="                                                                   " lineBreakMode="tailTruncation" baselineAdjustment="alignBaselines" adjustsFontSizeToFit="NO" translatesAutoresizingMaskIntoConstraints="NO" id="cTX-cU-wH6">
181	+                                        <rect key="frame" x="-1" y="224" width="322" height="5"/>
182	+                                        <autoresizingMask key="autoresizingMask" flexibleMaxX="YES" flexibleMaxY="YES"/>
183	+                                        <color key="backgroundColor" white="0.0" alpha="1" colorSpace="calibratedWhite"/>
184	+                                        <fontDescription key="fontDescription" type="system" pointSize="17"/>
185	+                                        <nil key="highlightedColor"/>
186	+                                    </label>
187	+                                    <label opaque="NO" clipsSubviews="YES" userInteractionEnabled="NO" contentMode="left" horizontalHuggingPriority="251" verticalHuggingPriority="251" fixedFrame="YES" text="NSNumber" lineBreakMode="tailTruncation" baselineAdjustment="alignBaselines" adjustsFontSizeToFit="NO" translatesAutoresizingMaskIntoConstraints="NO" id="0gL-lq-eCC">
188	+                                        <rect key="frame" x="15" y="241" width="85" height="21"/>
189	+                                        <autoresizingMask key="autoresizingMask" flexibleMaxX="YES" flexibleMaxY="YES"/>
190	+                                        <fontDescription key="fontDescription" type="system" pointSize="17"/>
191	+                                        <color key="textColor" cocoaTouchSystemColor="darkTextColor"/>
192	+                                        <nil key="highlightedColor"/>
193	+                                    </label>
194	+                                    <button opaque="NO" contentMode="scaleToFill" fixedFrame="YES" contentHorizontalAlignment="center" contentVerticalAlignment="center" buttonType="roundedRect" lineBreakMode="middleTruncation" translatesAutoresizingMaskIntoConstraints="NO" id="KGG-yb-GNo">
195	+                                        <rect key="frame" x="108" y="237" width="33" height="30"/>
196	+                                        <autoresizingMask key="autoresizingMask" flexibleMaxX="YES" flexibleMaxY="YES"/>
197	+                                        <state key="normal" title="wipe">
198	+                                            <color key="titleShadowColor" white="0.5" alpha="1" colorSpace="calibratedWhite"/>
199	+                                        </state>
200	+                                        <connections>
201	+                                            <action selector="NumberWipe:" destination="2" eventType="touchUpInside" id="ctv-GI-Wg7"/>
202	+                                        </connections>
203	+                                    </button>
204	+                                    <button opaque="NO" contentMode="scaleToFill" fixedFrame="YES" contentHorizontalAlignment="center" contentVerticalAlignment="center" buttonType="roundedRect" lineBreakMode="middleTruncation" translatesAutoresizingMaskIntoConstraints="NO" id="ifd-Ge-gsu">
205	+                                        <rect key="frame" x="225" y="237" width="30" height="30"/>
206	+                                        <autoresizingMask key="autoresizingMask" flexibleMaxX="YES" flexibleMaxY="YES"/>
207	+                                        <state key="normal" title="lock">
208	+                                            <color key="titleShadowColor" white="0.5" alpha="1" colorSpace="calibratedWhite"/>
209	+                                        </state>
210	+                                        <connections>
211	+                                            <action selector="NumberLock:" destination="2" eventType="touchUpInside" id="zzY-w9-4Qs"/>
212	+                                        </connections>
213	+                                    </button>
214	+                                    <button opaque="NO" contentMode="scaleToFill" fixedFrame="YES" contentHorizontalAlignment="center" contentVerticalAlignment="center" buttonType="roundedRect" lineBreakMode="middleTruncation" translatesAutoresizingMaskIntoConstraints="NO" id="bIh-fV-cpP">
215	+                                        <rect key="frame" x="266" y="237" width="46" height="30"/>
216	+                                        <autoresizingMask key="autoresizingMask" flexibleMaxX="YES" flexibleMaxY="YES"/>
217	+                                        <state key="normal" title="unlock">
218	+                                            <color key="titleShadowColor" white="0.5" alpha="1" colorSpace="calibratedWhite"/>
219	+                                        </state>
220	+                                        <connections>
221	+                                            <action selector="NumberUnlock:" destination="2" eventType="touchUpInside" id="ECc-bY-S9S"/>
222	+                                        </connections>
223	+                                    </button>
224	+                                    <button opaque="NO" contentMode="scaleToFill" fixedFrame="YES" contentHorizontalAlignment="center" contentVerticalAlignment="center" buttonType="roundedRect" lineBreakMode="middleTruncation" translatesAutoresizingMaskIntoConstraints="NO" id="wZZ-bb-3NJ">
225	+                                        <rect key="frame" x="149" y="237" width="61" height="30"/>
226	+                                        <autoresizingMask key="autoresizingMask" flexibleMaxX="YES" flexibleMaxY="YES"/>
227	+                                        <state key="normal" title="track">
228	+                                            <color key="titleShadowColor" white="0.5" alpha="1" colorSpace="calibratedWhite"/>
229	+                                        </state>
230	+                                        <connections>
231	+                                            <action selector="NumberTrack:" destination="2" eventType="touchUpInside" id="sNT-z2-JWZ"/>
232	+                                        </connections>
233	+                                    </button>
234	+                                    <label opaque="NO" clipsSubviews="YES" userInteractionEnabled="NO" contentMode="left" horizontalHuggingPriority="251" verticalHuggingPriority="251" fixedFrame="YES" text="NumLabel" lineBreakMode="tailTruncation" baselineAdjustment="alignBaselines" adjustsFontSizeToFit="NO" translatesAutoresizingMaskIntoConstraints="NO" id="dMv-Nv-81C">
235	+                                        <rect key="frame" x="15" y="270" width="293" height="21"/>
236	+                                        <autoresizingMask key="autoresizingMask" flexibleMaxX="YES" flexibleMaxY="YES"/>
237	+                                        <fontDescription key="fontDescription" type="system" pointSize="17"/>
238	+                                        <nil key="highlightedColor"/>
239	+                                    </label>
240	+                                    <label opaque="NO" clipsSubviews="YES" userInteractionEnabled="NO" contentMode="left" horizontalHuggingPriority="251" verticalHuggingPriority="251" fixedFrame="YES" text="NumHex" lineBreakMode="tailTruncation" baselineAdjustment="alignBaselines" adjustsFontSizeToFit="NO" translatesAutoresizingMaskIntoConstraints="NO" id="SFZ-y2-4K6">
241	+                                        <rect key="frame" x="15" y="299" width="293" height="21"/>
242	+                                        <autoresizingMask key="autoresizingMask" flexibleMaxX="YES" flexibleMaxY="YES"/>
243	+                                        <fontDescription key="fontDescription" name="Courier" family="Courier" pointSize="12"/>
244	+                                        <nil key="highlightedColor"/>
245	+                                    </label>
246	+                                    <label opaque="NO" clipsSubviews="YES" userInteractionEnabled="NO" contentMode="left" horizontalHuggingPriority="251" verticalHuggingPriority="251" fixedFrame="YES" text="                                                                   " lineBreakMode="tailTruncation" baselineAdjustment="alignBaselines" adjustsFontSizeToFit="NO" translatesAutoresizingMaskIntoConstraints="NO" id="LFS-gu-Ug4">
247	+                                        <rect key="frame" x="0.0" y="328" width="322" height="5"/>
248	+                                        <autoresizingMask key="autoresizingMask" flexibleMaxX="YES" flexibleMaxY="YES"/>
249	+                                        <color key="backgroundColor" white="0.0" alpha="1" colorSpace="calibratedWhite"/>
250	+                                        <fontDescription key="fontDescription" type="system" pointSize="17"/>
251	+                                        <nil key="highlightedColor"/>
252	+                                    </label>
253	+                                    <label opaque="NO" clipsSubviews="YES" userInteractionEnabled="NO" contentMode="left" horizontalHuggingPriority="251" verticalHuggingPriority="251" fixedFrame="YES" text="NSArray" lineBreakMode="tailTruncation" baselineAdjustment="alignBaselines" adjustsFontSizeToFit="NO" translatesAutoresizingMaskIntoConstraints="NO" id="Im0-j7-Nq0">
254	+                                        <rect key="frame" x="15" y="345" width="64" height="21"/>
255	+                                        <autoresizingMask key="autoresizingMask" flexibleMaxX="YES" flexibleMaxY="YES"/>
256	+                                        <fontDescription key="fontDescription" type="system" pointSize="17"/>
257	+                                        <color key="textColor" cocoaTouchSystemColor="darkTextColor"/>
258	+                                        <nil key="highlightedColor"/>
259	+                                    </label>
260	+                                    <button opaque="NO" contentMode="scaleToFill" fixedFrame="YES" contentHorizontalAlignment="center" contentVerticalAlignment="center" buttonType="roundedRect" lineBreakMode="middleTruncation" translatesAutoresizingMaskIntoConstraints="NO" id="nWZ-YH-ZW6">
261	+                                        <rect key="frame" x="108" y="341" width="33" height="30"/>
262	+                                        <autoresizingMask key="autoresizingMask" flexibleMaxX="YES" flexibleMaxY="YES"/>
263	+                                        <state key="normal" title="wipe">
264	+                                            <color key="titleShadowColor" white="0.5" alpha="1" colorSpace="calibratedWhite"/>
265	+                                        </state>
266	+                                        <connections>
267	+                                            <action selector="ArrayWipe:" destination="2" eventType="touchUpInside" id="peq-Id-jUA"/>
268	+                                        </connections>
269	+                                    </button>
270	+                                    <button opaque="NO" contentMode="scaleToFill" fixedFrame="YES" contentHorizontalAlignment="center" contentVerticalAlignment="center" buttonType="roundedRect" lineBreakMode="middleTruncation" translatesAutoresizingMaskIntoConstraints="NO" id="AsD-Sb-S86">
271	+                                        <rect key="frame" x="225" y="341" width="30" height="30"/>
272	+                                        <autoresizingMask key="autoresizingMask" flexibleMaxX="YES" flexibleMaxY="YES"/>
273	+                                        <state key="normal" title="lock">
274	+                                            <color key="titleShadowColor" white="0.5" alpha="1" colorSpace="calibratedWhite"/>
275	+                                        </state>
276	+                                        <connections>
277	+                                            <action selector="ArrayLock:" destination="2" eventType="touchUpInside" id="cco-N9-7ta"/>
278	+                                        </connections>
279	+                                    </button>
280	+                                    <button opaque="NO" contentMode="scaleToFill" fixedFrame="YES" contentHorizontalAlignment="center" contentVerticalAlignment="center" buttonType="roundedRect" lineBreakMode="middleTruncation" translatesAutoresizingMaskIntoConstraints="NO" id="1cg-i9-DAI">
281	+                                        <rect key="frame" x="266" y="341" width="46" height="30"/>
282	+                                        <autoresizingMask key="autoresizingMask" flexibleMaxX="YES" flexibleMaxY="YES"/>
283	+                                        <state key="normal" title="unlock">
284	+                                            <color key="titleShadowColor" white="0.5" alpha="1" colorSpace="calibratedWhite"/>
285	+                                        </state>
286	+                                        <connections>
287	+                                            <action selector="ArrayUnlock:" destination="2" eventType="touchUpInside" id="lrk-xt-R7K"/>
288	+                                        </connections>
289	+                                    </button>
290	+                                    <button opaque="NO" contentMode="scaleToFill" fixedFrame="YES" contentHorizontalAlignment="center" contentVerticalAlignment="center" buttonType="roundedRect" lineBreakMode="middleTruncation" translatesAutoresizingMaskIntoConstraints="NO" id="Any-Rn-8Sb">
291	+                                        <rect key="frame" x="149" y="341" width="61" height="30"/>
292	+                                        <autoresizingMask key="autoresizingMask" flexibleMaxX="YES" flexibleMaxY="YES"/>
293	+                                        <state key="normal" title="track">
294	+                                            <color key="titleShadowColor" white="0.5" alpha="1" colorSpace="calibratedWhite"/>
295	+                                        </state>
296	+                                        <connections>
297	+                                            <action selector="ArrayTrack:" destination="2" eventType="touchUpInside" id="3fr-vv-dRU"/>
298	+                                        </connections>
299	+                                    </button>
300	+                                    <label opaque="NO" clipsSubviews="YES" userInteractionEnabled="NO" contentMode="left" horizontalHuggingPriority="251" verticalHuggingPriority="251" fixedFrame="YES" text="ArrayLabel" lineBreakMode="tailTruncation" baselineAdjustment="alignBaselines" adjustsFontSizeToFit="NO" translatesAutoresizingMaskIntoConstraints="NO" id="9nm-RG-WT7">
301	+                                        <rect key="frame" x="15" y="374" width="293" height="21"/>
302	+                                        <autoresizingMask key="autoresizingMask" flexibleMaxX="YES" flexibleMaxY="YES"/>
303	+                                        <fontDescription key="fontDescription" type="system" pointSize="12"/>
304	+                                        <nil key="highlightedColor"/>
305	+                                    </label>
306	+                                </subviews>
307	+                            </scrollView>
445	308	                         </subviews>
446	309	                         <color key="backgroundColor" white="1" alpha="1" colorSpace="custom" customColorSpace="calibratedWhite"/>
447		-                        <constraints>
448		-                            <constraint firstItem="47A-8u-V1R" firstAttribute="leading" secondItem="P7g-Ha-dBr" secondAttribute="leading" type="default" id="0FK-L4-R0f"/>
449		-                            <constraint firstItem="y86-FI-t8w" firstAttribute="top" secondItem="YBo-gW-lDk" secondAttribute="top" type="default" id="0Hd-TT-HCL"/>
450		-                            <constraint firstItem="haZ-1C-gLf" firstAttribute="trailing" secondItem="FdT-JW-BaB" secondAttribute="trailing" type="default" id="0sI-Wm-8hj"/>
451		-                            <constraint firstItem="47A-8u-V1R" firstAttribute="bottom" secondItem="yPn-Yt-de3" secondAttribute="bottom" type="default" id="11E-DA-paM"/>
452		-                            <constraint firstItem="47A-8u-V1R" firstAttribute="trailing" secondItem="P7g-Ha-dBr" secondAttribute="trailing" type="default" id="12w-GP-dIn"/>
453		-                            <constraint firstItem="ETE-vt-zWY" firstAttribute="bottom" secondItem="P7g-Ha-dBr" secondAttribute="bottom" type="default" id="27v-lR-WPz"/>
454		-                            <constraint firstItem="G5L-hc-uEX" firstAttribute="leading" secondItem="3" secondAttribute="leading" constant="27" id="2tM-J3-BNW"/>
455		-                            <constraint firstItem="qYb-w8-oEj" firstAttribute="leading" secondItem="xLN-TM-gKU" secondAttribute="leading" type="default" id="3Jx-wc-rLB"/>
456		-                            <constraint firstItem="xLN-TM-gKU" firstAttribute="trailing" secondItem="Gu9-eK-rVY" secondAttribute="trailing" type="default" id="4Az-yU-c2E"/>
457		-                            <constraint firstItem="Atv-XN-z4x" firstAttribute="top" secondItem="lN4-ps-aIf" secondAttribute="bottom" constant="8" symbolic="YES" type="default" id="6Y6-p5-Apz"/>
458		-                            <constraint firstItem="dpm-HB-IJT" firstAttribute="leading" secondItem="u1c-dm-6ud" secondAttribute="leading" type="default" id="6tJ-Js-5pg"/>
459		-                            <constraint firstItem="lvZ-lv-UPk" firstAttribute="top" secondItem="d0F-qV-STH" secondAttribute="bottom" constant="8" symbolic="YES" type="default" id="7Jt-VH-OXh"/>
460		-                            <constraint firstItem="lvZ-lv-UPk" firstAttribute="trailing" secondItem="lBU-4d-AnD" secondAttribute="trailing" type="default" id="7nJ-1Z-83V"/>
461		-                            <constraint firstItem="Atv-XN-z4x" firstAttribute="bottom" secondItem="uPq-tp-wen" secondAttribute="bottom" type="default" id="8az-5F-VSu"/>
462		-                            <constraint firstItem="37q-JP-ijS" firstAttribute="bottom" secondItem="3" secondAttribute="bottom" type="default" id="B2q-31-8on"/>
463		-                            <constraint firstItem="Kjl-mI-E8q" firstAttribute="leading" secondItem="xLN-TM-gKU" secondAttribute="leading" type="default" id="BDS-U1-FGF"/>
464		-                            <constraint firstItem="Jv9-P4-E8a" firstAttribute="top" secondItem="FdT-JW-BaB" secondAttribute="bottom" constant="8" symbolic="YES" type="default" id="C8h-d0-NQH"/>
465		-                            <constraint firstItem="lBU-4d-AnD" firstAttribute="trailing" secondItem="r7R-D1-lVt" secondAttribute="trailing" type="default" id="CVt-DP-xEq"/>
466		-                            <constraint firstItem="2H6-VV-Dvf" firstAttribute="leading" secondItem="Gu9-eK-rVY" secondAttribute="leading" type="default" id="Cem-c1-mXq"/>
467		-                            <constraint firstItem="Wdl-BB-pz1" firstAttribute="centerX" secondItem="Gu9-eK-rVY" secondAttribute="centerX" type="default" id="CyH-ST-M99"/>
468		-                            <constraint firstItem="GmH-vb-QuB" firstAttribute="top" secondItem="2oS-th-M8i" secondAttribute="bottom" constant="8" symbolic="YES" type="default" id="D1S-IE-Yzc"/>
469		-                            <constraint firstItem="XEw-Hc-TyQ" firstAttribute="leading" secondItem="YBo-gW-lDk" secondAttribute="trailing" constant="8" symbolic="YES" type="default" id="E2J-QL-4ip"/>
470		-                            <constraint firstItem="GmH-vb-QuB" firstAttribute="baseline" secondItem="6tP-Vr-jxY" secondAttribute="baseline" type="default" id="Enc-UA-SgQ"/>
471		-                            <constraint firstItem="xLN-TM-gKU" firstAttribute="top" secondItem="G5L-hc-uEX" secondAttribute="bottom" constant="8" symbolic="YES" type="default" id="FMj-18-0XB"/>
472		-                            <constraint firstItem="haZ-1C-gLf" firstAttribute="leading" secondItem="3" secondAttribute="leading" constant="20" symbolic="YES" type="default" id="GMa-wc-TcS"/>
473		-                            <constraint firstItem="37q-JP-ijS" firstAttribute="trailing" secondItem="r7R-D1-lVt" secondAttribute="trailing" type="default" id="GjQ-cN-ffl"/>
474		-                            <constraint firstItem="YBo-gW-lDk" firstAttribute="leading" secondItem="Jv9-P4-E8a" secondAttribute="leading" type="default" id="Gqh-d7-0WI"/>
475		-                            <constraint firstItem="G5L-hc-uEX" firstAttribute="trailing" secondItem="dpm-HB-IJT" secondAttribute="trailing" type="default" id="Hsk-ps-LfI"/>
476		-                            <constraint firstItem="y86-FI-t8w" firstAttribute="leading" secondItem="3" secondAttribute="leading" constant="55" id="IHf-1Z-j6e"/>
477		-                            <constraint firstItem="37q-JP-ijS" firstAttribute="leading" secondItem="r7R-D1-lVt" secondAttribute="leading" type="default" id="KpI-ic-jbc"/>
478		-                            <constraint firstItem="haZ-1C-gLf" firstAttribute="top" secondItem="3" secondAttribute="top" constant="55" id="Lo6-Sd-x3s"/>
479		-                            <constraint firstItem="47A-8u-V1R" firstAttribute="top" secondItem="yPn-Yt-de3" secondAttribute="top" type="default" id="M3N-zx-0qI"/>
480		-                            <constraint firstItem="Kjl-mI-E8q" firstAttribute="leading" secondItem="haZ-1C-gLf" secondAttribute="leading" type="default" id="M3x-fs-t3w"/>
481		-                            <constraint firstItem="YBo-gW-lDk" firstAttribute="baseline" secondItem="XEw-Hc-TyQ" secondAttribute="baseline" type="default" id="N5z-Eb-9k8"/>
482		-                            <constraint firstItem="uPq-tp-wen" firstAttribute="trailing" secondItem="AEQ-bX-01b" secondAttribute="trailing" type="default" id="N88-HM-qMY"/>
483		-                            <constraint firstItem="y86-FI-t8w" firstAttribute="top" secondItem="u1c-dm-6ud" secondAttribute="bottom" constant="8" symbolic="YES" type="default" id="Nl4-2F-PCh"/>
484		-                            <constraint firstItem="AEQ-bX-01b" firstAttribute="top" secondItem="lN4-ps-aIf" secondAttribute="top" type="default" id="O0F-PA-hN7"/>
485		-                            <constraint firstItem="dWj-7L-KOU" firstAttribute="top" secondItem="3" secondAttribute="top" constant="14" id="P1t-kk-Pl4"/>
486		-                            <constraint firstItem="G5L-hc-uEX" firstAttribute="centerY" secondItem="3" secondAttribute="centerY" type="default" id="PAf-a1-0g9"/>
487		-                            <constraint firstAttribute="trailing" secondItem="lvZ-lv-UPk" secondAttribute="trailing" type="default" id="QPK-ys-7U2"/>
488		-                            <constraint firstAttribute="bottom" secondItem="P7g-Ha-dBr" secondAttribute="bottom" constant="151" id="RHS-RN-Q2G"/>
489		-                            <constraint firstItem="Kjl-mI-E8q" firstAttribute="trailing" secondItem="Gu9-eK-rVY" secondAttribute="trailing" type="default" id="RWq-Ae-v0y"/>
490		-                            <constraint firstItem="FdT-JW-BaB" firstAttribute="top" secondItem="3" secondAttribute="top" constant="88" id="Rza-KY-9EN"/>
491		-                            <constraint firstItem="Kjl-mI-E8q" firstAttribute="top" secondItem="y86-FI-t8w" secondAttribute="bottom" constant="8" symbolic="YES" type="default" id="SUD-jl-wz0"/>
492		-                            <constraint firstItem="lN4-ps-aIf" firstAttribute="baseline" secondItem="AEQ-bX-01b" secondAttribute="baseline" type="default" id="Shz-zC-irq"/>
493		-                            <constraint firstItem="ETE-vt-zWY" firstAttribute="leading" secondItem="yPn-Yt-de3" secondAttribute="leading" type="default" id="T6g-qo-hzL"/>
494		-                            <constraint firstItem="P7g-Ha-dBr" firstAttribute="leading" secondItem="qYb-w8-oEj" secondAttribute="leading" type="default" id="TpU-V0-otG"/>
495		-                            <constraint firstItem="2oS-th-M8i" firstAttribute="top" secondItem="3" secondAttribute="top" constant="178" id="V9c-a2-TrU"/>
496		-                            <constraint firstAttribute="bottom" secondItem="lBU-4d-AnD" secondAttribute="bottom" constant="45" id="VOH-za-aZO"/>
497		-                            <constraint firstItem="GmH-vb-QuB" firstAttribute="leading" secondItem="XEw-Hc-TyQ" secondAttribute="leading" type="default" id="Vtx-LE-9Cw"/>
498		-                            <constraint firstItem="lvZ-lv-UPk" firstAttribute="leading" secondItem="lBU-4d-AnD" secondAttribute="leading" type="default" id="WFM-NA-PzD"/>
499		-                            <constraint firstAttribute="bottom" secondItem="47A-8u-V1R" secondAttribute="bottom" constant="128" id="WM2-Rg-fd4"/>
500		-                            <constraint firstItem="dpm-HB-IJT" firstAttribute="top" secondItem="2oS-th-M8i" secondAttribute="bottom" constant="8" symbolic="YES" type="default" id="WVa-t8-liU"/>
501		-                            <constraint firstItem="Kjl-mI-E8q" firstAttribute="trailing" secondItem="FdT-JW-BaB" secondAttribute="trailing" type="default" id="X8T-52-dOz"/>
502		-                            <constraint firstItem="uPq-tp-wen" firstAttribute="top" secondItem="AEQ-bX-01b" secondAttribute="bottom" constant="8" symbolic="YES" type="default" id="XhS-lu-U2y"/>
503		-                            <constraint firstItem="r7R-D1-lVt" firstAttribute="leading" secondItem="2H6-VV-Dvf" secondAttribute="leading" type="default" id="Yre-0S-3EY"/>
504		-                            <constraint firstItem="dpm-HB-IJT" firstAttribute="bottom" secondItem="Wdl-BB-pz1" secondAttribute="bottom" type="default" id="aKU-Bi-0zv"/>
505		-                            <constraint firstItem="Jv9-P4-E8a" firstAttribute="leading" secondItem="3" secondAttribute="leading" constant="135" id="aZc-ku-Mq1"/>
506		-                            <constraint firstItem="AEQ-bX-01b" firstAttribute="leading" secondItem="3" secondAttribute="leading" constant="140" id="abi-Tx-Zea"/>
507		-                            <constraint firstItem="dWj-7L-KOU" firstAttribute="trailing" secondItem="haZ-1C-gLf" secondAttribute="trailing" type="default" id="atY-wy-GoI"/>
508		-                            <constraint firstItem="Kjl-mI-E8q" firstAttribute="top" secondItem="YBo-gW-lDk" secondAttribute="bottom" constant="8" symbolic="YES" type="default" id="bHR-qM-UbZ"/>
509		-                            <constraint firstItem="r7R-D1-lVt" firstAttribute="bottom" secondItem="37q-JP-ijS" secondAttribute="top" type="default" id="dbR-6Y-HsS"/>
510		-                            <constraint firstItem="XEw-Hc-TyQ" firstAttribute="leading" secondItem="Jv9-P4-E8a" secondAttribute="trailing" constant="8" symbolic="YES" type="default" id="e8I-Pd-2Oj"/>
511		-                            <constraint firstItem="XEw-Hc-TyQ" firstAttribute="top" secondItem="3" secondAttribute="top" constant="104" id="e9N-tQ-LDc"/>
512		-                            <constraint firstItem="FdT-JW-BaB" firstAttribute="leading" secondItem="Gu9-eK-rVY" secondAttribute="leading" type="default" id="fMG-Z7-fjz"/>
513		-                            <constraint firstItem="6tP-Vr-jxY" firstAttribute="trailing" secondItem="Wdl-BB-pz1" secondAttribute="trailing" type="default" id="gbc-lm-IQV"/>
514		-                            <constraint firstItem="d0F-qV-STH" firstAttribute="top" secondItem="qYb-w8-oEj" secondAttribute="bottom" constant="8" symbolic="YES" type="default" id="gp5-0r-fCL"/>
515		-                            <constraint firstItem="dpm-HB-IJT" firstAttribute="trailing" secondItem="u1c-dm-6ud" secondAttribute="trailing" type="default" id="gx7-pL-uXe"/>
516		-                            <constraint firstItem="47A-8u-V1R" firstAttribute="leading" secondItem="lvZ-lv-UPk" secondAttribute="leading" type="default" id="h7g-eb-od6"/>
517		-                            <constraint firstItem="P7g-Ha-dBr" firstAttribute="top" secondItem="2H6-VV-Dvf" secondAttribute="bottom" constant="8" symbolic="YES" type="default" id="jMW-eY-8yU"/>
518		-                            <constraint firstItem="GmH-vb-QuB" firstAttribute="trailing" secondItem="XEw-Hc-TyQ" secondAttribute="trailing" type="default" id="jbQ-QC-Blb"/>
519		-                            <constraint firstItem="lN4-ps-aIf" firstAttribute="leading" secondItem="3" secondAttribute="leading" constant="37" id="jj7-ce-RTI"/>
520		-                            <constraint firstItem="dpm-HB-IJT" firstAttribute="top" secondItem="Gu9-eK-rVY" secondAttribute="bottom" constant="8" symbolic="YES" type="default" id="kKd-S3-cgk"/>
521		-                            <constraint firstItem="d0F-qV-STH" firstAttribute="leading" secondItem="ETE-vt-zWY" secondAttribute="trailing" constant="8" symbolic="YES" type="default" id="kb8-FR-IVn"/>
522		-                            <constraint firstItem="Wdl-BB-pz1" firstAttribute="top" secondItem="Gu9-eK-rVY" secondAttribute="bottom" constant="8" symbolic="YES" type="default" id="l4P-At-ABb"/>
523		-                            <constraint firstItem="6tP-Vr-jxY" firstAttribute="leading" secondItem="Wdl-BB-pz1" secondAttribute="leading" type="default" id="mWe-AG-c9b"/>
524		-                            <constraint firstItem="uPq-tp-wen" firstAttribute="leading" secondItem="AEQ-bX-01b" secondAttribute="leading" type="default" id="peI-nU-KXX"/>
525		-                            <constraint firstItem="37q-JP-ijS" firstAttribute="leading" secondItem="3" secondAttribute="leading" type="default" id="rKr-E0-vWn"/>
526		-                            <constraint firstItem="ETE-vt-zWY" firstAttribute="top" secondItem="2H6-VV-Dvf" secondAttribute="bottom" constant="8" symbolic="YES" type="default" id="sA5-49-uiz"/>
527		-                            <constraint firstItem="G5L-hc-uEX" firstAttribute="leading" secondItem="dpm-HB-IJT" secondAttribute="leading" type="default" id="sTP-fp-7Kh"/>
528		-                            <constraint firstItem="lN4-ps-aIf" firstAttribute="top" secondItem="3" secondAttribute="top" constant="2" id="tJM-ej-kqt"/>
529		-                            <constraint firstItem="d0F-qV-STH" firstAttribute="leading" secondItem="yPn-Yt-de3" secondAttribute="trailing" constant="8" symbolic="YES" type="default" id="tKC-PE-kY6"/>
530		-                            <constraint firstItem="ETE-vt-zWY" firstAttribute="leading" secondItem="3" secondAttribute="leading" constant="100" id="tZZ-HU-zJo"/>
531		-                            <constraint firstItem="lvZ-lv-UPk" firstAttribute="trailing" secondItem="2H6-VV-Dvf" secondAttribute="trailing" type="default" id="tdK-al-XTk"/>
532		-                            <constraint firstItem="lN4-ps-aIf" firstAttribute="leading" secondItem="Atv-XN-z4x" secondAttribute="leading" type="default" id="ucF-fQ-SNK"/>
533		-                            <constraint firstItem="lN4-ps-aIf" firstAttribute="trailing" secondItem="Atv-XN-z4x" secondAttribute="trailing" type="default" id="ueY-eW-RuT"/>
534		-                            <constraint firstItem="qYb-w8-oEj" firstAttribute="trailing" secondItem="2H6-VV-Dvf" secondAttribute="trailing" type="default" id="vdG-h8-V7c"/>
535		-                            <constraint firstItem="qYb-w8-oEj" firstAttribute="trailing" secondItem="xLN-TM-gKU" secondAttribute="trailing" type="default" id="wpn-U9-9Rd"/>
536		-                            <constraint firstAttribute="bottom" secondItem="lvZ-lv-UPk" secondAttribute="bottom" constant="99" id="zN4-rJ-0Cy"/>
537		-                            <constraint firstItem="Gu9-eK-rVY" firstAttribute="centerX" secondItem="2oS-th-M8i" secondAttribute="centerX" type="default" id="zqb-4Q-3Ev"/>
538		-                        </constraints>
539	310	                     </view>
540	311	                     <connections>
541		-                        <outlet property="ArrTrackButton" destination="Atv-XN-z4x" id="F23-LF-KGJ"/>
542		-                        <outlet property="ArrayLabel" destination="haZ-1C-gLf" id="ol3-Ll-fuY"/>
543		-                        <outlet property="DataHex" destination="qYb-w8-oEj" id="B36-u5-0zg"/>
544		-                        <outlet property="DataLabel" destination="xLN-TM-gKU" id="wfr-uy-SEf"/>
545		-                        <outlet property="DataTrackButton" destination="G5L-hc-uEX" id="da3-V9-0PV"/>
546		-                        <outlet property="NumHex" destination="lBU-4d-AnD" id="5fL-0q-Kuu"/>
547		-                        <outlet property="NumLabel" destination="lvZ-lv-UPk" id="6TG-gh-gbz"/>
548		-                        <outlet property="NumTrackButton" destination="47A-8u-V1R" id="sWS-cD-eNK"/>
549		-                        <outlet property="StrHex" destination="2oS-th-M8i" id="aJp-pN-6dp"/>
550		-                        <outlet property="StrLabel" destination="Kjl-mI-E8q" id="OYg-I2-9ci"/>
551		-                        <outlet property="StrTrackButton" destination="y86-FI-t8w" id="uvf-fw-hoq"/>
312	+                        <outlet property="ArrTrackButton" destination="Any-Rn-8Sb" id="6gs-Qi-uId"/>
313	+                        <outlet property="ArrayLabel" destination="9nm-RG-WT7" id="1Ty-f4-iha"/>
314	+                        <outlet property="DataHex" destination="xRQ-ZY-YJl" id="JgY-DT-oTT"/>
315	+                        <outlet property="DataLabel" destination="B1u-7b-1Aq" id="UpV-lb-0Xl"/>
316	+                        <outlet property="DataTrackButton" destination="Qtb-hp-9kW" id="azy-NG-GOz"/>
317	+                        <outlet property="ExitButton" destination="b03-L3-ykn" id="Tl1-cT-cO6"/>
318	+                        <outlet property="NumHex" destination="SFZ-y2-4K6" id="l9N-EW-FDS"/>
319	+                        <outlet property="NumLabel" destination="dMv-Nv-81C" id="3lO-ui-nA3"/>
320	+                        <outlet property="NumTrackButton" destination="wZZ-bb-3NJ" id="XE5-fk-OcX"/>
321	+                        <outlet property="StrHex" destination="ZfG-il-4O9" id="rZC-S3-f8Z"/>
322	+                        <outlet property="StrLabel" destination="KRd-cw-0TM" id="m7R-xP-msy"/>
323	+                        <outlet property="StrTrackButton" destination="omn-rx-RLc" id="zoa-5S-t5Y"/>
552	324	                     </connections>
553	325	                 </viewController>
554	326	                 <placeholder placeholderIdentifier="IBFirstResponder" id="4" sceneMemberID="firstResponder"/>
555	327	             </objects>
328	+            <point key="canvasLocation" x="238" y="138"/>
556	329	         </scene>
557	330	     </scenes>
558	331	     <simulatedMetricsContainer key="defaultSimulatedMetrics">
559	332	         <simulatedStatusBarMetrics key="statusBar"/>
560	333	         <simulatedOrientationMetrics key="orientation"/>
561		-        <simulatedScreenMetrics key="destination" type="retina4"/>
334	+        <simulatedScreenMetrics key="destination"/>
562	335	     </simulatedMetricsContainer>
563	336	 </document>
