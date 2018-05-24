# Test video sequences for stationary object detection and abandoned & stolen object classification

This data set contains 14 video sequences and ground truth files for stationary foreground segmentation tasks and abandoned & stolen object detection.

## Sequences
<table style="undefined;table-layout: fixed; width: 457px"><colgroup><col style="width: 114px"><col style="width: 163px"><col style="width: 86px"><col style="width: 94px"></colgroup><tr><th>Sequence</th><th>Source</th><th colspan="2">Stationary objects</th></tr><tr><td>VISOR_00</td><td>visor_Video00<br>1:2308</td><td>720:2308<br>875:1610</td><td>car #1<br>car #2</td></tr><tr><td>VISOR_01</td><td>visor_Video01<br>1:3330</td><td>970:2720</td><td>car</td></tr><tr><td>VISOR_02</td><td>visor_Video02<br>1:2815</td><td>850:2700<br>1530:2710</td><td>car #1<br>car #2</td></tr><tr><td>VISOR_03</td><td>visor_Video03<br>1:3075</td><td>975:2385</td><td>car</td></tr><tr><td>AVSS_00a</td><td>AVSSS07_EASY<br>1500:3775</td><td>500:2275</td><td>suitcase</td></tr><tr><td>AVSS_00b</td><td>AVSSS07_EASY<br>3780:5465</td><td>1:1100</td><td>suitcase</td></tr><tr><td>AVSS_01a</td><td>AVSSS07_MEDIUM<br>1:3000</td><td>1410:3000</td><td>bag</td></tr><tr><td>AVSS_01b</td><td>AVSSS07_MEDIUM<br>2880:4812</td><td>1:1650</td><td>bag</td></tr><tr><td>PETS_00a</td><td>PETS2006_S1_C3<br>1:2992</td><td>1890:2992</td><td>bag</td></tr><tr><td>PETS_00b</td><td>PETS2006_S1_C3<br>2992:1</td><td>1:1190</td><td>bag</td></tr><tr><td>PETS_01a</td><td>PETS2006_S4_C3<br>1:3052</td><td>840:3052</td><td>suitcase</td></tr><tr><td>PETS_01b</td><td>PETS2006_S4_C3<br>3052:1</td><td>1:2265</td><td>suitcase</td></tr><tr><td>PETS_02a</td><td>PETS2006_S5_C3<br>1:3361</td><td>1860:3361</td><td>plank</td></tr><tr><td>PETS_02b</td><td>PETS2006_S5_C3<br>3361:1</td><td>1:1590</td><td>plank</td></tr></table>

## Ground truth files
Ground truth files are comma separated text files. For every frame containing a stationay object the ground truth file contains a row starting with the frame index (from 1) and then for each blob of the frame the bounding box and class (abandoned / stolen) is given.

E.g. for two blobs
```
frame;x1,y1,w1,h1,C1;x2,y2,w2,h2,C2;
```
where `frame` is the frame index, the blob descriptions are also spearated with `;` and the blob description gives the $$x$$ , $$y$$ coordinates and width, hegith. The label ob the blob can be `A` if abandoned or `S` if stolen.

## Sources
The test videos used in this data set are from the VISOR, AVSS2007 and PETS2006 sets.
