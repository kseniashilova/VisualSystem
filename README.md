## Medulla  
Обработка визуальной информации drosophila melangoster берет свое начало в части глаза называемой retina, а затем первый из четырех нейропилей (neuropil) - частей оптической доли (optic lobe) - lamina - фиксирует сигнал с фоторецепторов.Затем сигнал проецируется во вторую область optic lobe, medulla. Medulla - это первый участок, где детектируется движение, сигнал, посылаемый в lobula plate, где нейроны интегрируют сигнал и посылают ответ на движение в зоне видимости.   
Более подробно процесс описан в статье [A visual motion detection circuit suggested by Drosophila connectomics](https://github.com/kseniashilova/SpikingNeuralNetwork/blob/main/A%20visual%20motion%20detection%20circuit%202.pdf).  
  
Именно потому, что medulla - это первый зависимый от motion-detection процесса нейропиль оптической части, интересно исследовать топологию частичного коннектома medulla.  
  
С помощью доступа к [Virtual Fly Brain](https://www.virtualflybrain.org/) из python (package vfb-connect) построим граф нейронов, которые находятся в medulla. 

Процесс в [python notebook](https://github.com/kseniashilova/VisualSystem/blob/main/VBF.ipynb).  
Результат визуализации региона medulla по слоям (M1, M2, M3, M4, M5, M6, M8, M9, M10) по данным, представленным в [Virtual Fly Brain](https://www.virtualflybrain.org/) в [файле](https://github.com/kseniashilova/VisualSystem/blob/main/optic_VBF2.html)    
![](https://github.com/kseniashilova/VisualSystem/blob/main/M1_M10_medulla.png) 
