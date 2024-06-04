# TBC-Classification
Thats my personal Project for exploring my knowledge of Machine Learning

I'm classified the TBC Bactery image using several architectures:
1. EfficientNet
2. SE-ResNet-18
3. GoogleNet
4. MobileNet
5. ResNet152 V2

## Requirements :
- pillow
- torch
- pandas
- matplotlib
- pickle
- torchvision
- efficientnet_pytorch
- scikit-learn
- seaborn

## Dataset
You can found Dataset TBC in [here](https://drive.google.com/drive/folders/1CwIdPFqb0a53i6O3lYEG_2ZYAuWGAPN2?usp=drive_link)

### Proportion TBC's Dataset :
<table>
  <tr>
    <th>Label Data</td>
    <th>Training Data</td>
    <th>Validation Data</td>
    <th>Testing Data</td>
  </tr>
  <tr>
    <td>**TBC**</td>
    <td>404</td>
    <td>101</td>
    <td>127</td>
  </tr>
  <tr>
    <td>**Non TBC**</td>
    <td>405</td>
    <td>102</td>
    <td>127</td>
  </tr>
</table>

## Preprocessing Image
- scaling with 224x224
- encode in pickle with dictionary format

## Performance
### Validation Performance
No	Model	loss(%)	Acc(%)	Precision(%)	Recall(%)	F1-Score(%)	time(s)	parameters
1	EfficientNet	9,20%	98,03%	98,04%	98,03%	98,03%	122,81	  4.010.110,00 
2	MobileNetV2	6,90%	97,04%	97,06%	97,05%	97,04%	76,88	  2.226.434,00 
3	GoogleNet	5,80%	98,52%	98,52%	98,52%	98,52%	76,04	  5.601.954,00 
4	ResNet152V2	10,44%	98,03%	98,04%	98,03%	98,03%	434,75	  58.147.906,00 
5	SE-ResNet-18	10,10%	97,54%	97,57%	97,54%	97,54%	67,90	  11.266.618,00 

### Testing Performance
No	Model	loss(%)	Acc(%)	Precision(%)	Recall(%)	F1-Score(%)	time(s)	parameters
1	EfficientNet	16,61%	97,24%	97,25%	97,24%	97,24%	122,81	  4.010.110 
2	MobileNetV2	11,88%	96,85%	96,85%	96,85%	96,85%	76,88	  2.226.434 
3	GoogleNet	9,74%	98,03%	98,06%	98,03%	98,03%	76,04	  5.601.954 
4	ResNet152V2	8,94%	97,24%	97,25%	97,24%	97,24%	434,75	  58.147.906 
5	SE-ResNet-18	6,63%	98,43%	98,44%	98,43%	98,43%	67,90	  11.266.618 

