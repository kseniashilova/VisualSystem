## Medulla  
Обработка визуальной информации drosophila melangoster берет свое начало в части глаза называемой retina, а затем первый из четырех нейропилей (neuropil) - частей оптической доли (optic lobe) - lamina - фиксирует сигнал с фоторецепторов.Затем сигнал проецируется во вторую область optic lobe, medulla. Medulla - это первый участок, где детектируется движение, сигнал, посылаемый в lobula plate, где нейроны интегрируют сигнал и посылают ответ на движение в зоне видимости.   
Более подробно процесс описан в статье [A visual motion detection circuit suggested by Drosophila connectomics](https://github.com/kseniashilova/SpikingNeuralNetwork/blob/main/A%20visual%20motion%20detection%20circuit%202.pdf).  
  
Именно потому, что medulla - это первый зависимый от motion-detection процесса нейропиль оптической части, интересно исследовать топологию частичного коннектома medulla.  
  
С помощью доступа к [Virtual Fly Brain](https://www.virtualflybrain.org/) из python (package vfb-connect) построим граф нейронов, которые находятся в medulla. 

Процесс в [python notebook](https://github.com/kseniashilova/VisualSystem/blob/main/VBF.ipynb).  
### Визуализация "малого" коннектома  
В статье [A visual motion detection circuit suggested by Drosophila connectomics](https://github.com/kseniashilova/SpikingNeuralNetwork/blob/main/A%20visual%20motion%20detection%20circuit%202.pdf) и нескольких других статьях об исследовании структуры региона medulla расматривается следующие нейроны и связи между ними:  
![](https://github.com/kseniashilova/VisualSystem/blob/main/pic/small_connectome.png)   
  
Похожий коннектом можно построить с помощью данных из [Virtual Fly Brain](https://www.virtualflybrain.org/). Чтобы быть точнее, нужно добавить к типам клеток, которые мы выделили из файла нейронов региона medulla, фоторецепторные клетки R7, R8. Это клетки региона lamina, именно поэтому их нет в файле, но для точного воспроизведения пути, отвечающему за детектирование движения, эти клетки необходимы.   
![](https://github.com/kseniashilova/VisualSystem/blob/main/pic/3_small_groups.jpg)    
  
   
 Коннектом разбит на 3 кластера (разбиение взято из данных [A visual motion detection circuit suggested by Drosophila connectomics](https://github.com/kseniashilova/SpikingNeuralNetwork/blob/main/A%20visual%20motion%20detection%20circuit%202.pdf)). Как можно увидеть, связи внутри нейронов фиолетового и зеленого кластера почти полностью повторяют схему из статьи, основные показанные связи. Что касается голубого кластера, результат похож на схему из статьи за исключением нескольких неточностей (отсутствие некоторых нейронов, добавление некоторых нейронов).   
Такая схема является наименьшей из возможных взятых подграфов коннектома medulla, по которой действительно возможно определить пути распространения сигнала, вызывающего ответ на даижение в широком поле.  
Результат визуализации региона medulla по слоям (M1, M2, M3, M4, M5, M6, M8, M9, M10) по данным, представленным в [Virtual Fly Brain](https://www.virtualflybrain.org/) в [файле](https://github.com/kseniashilova/VisualSystem/blob/main/optic_VBF2.html)    
![](https://github.com/kseniashilova/VisualSystem/blob/main/pic/M1_M10_medulla.png) 
