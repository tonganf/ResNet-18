## ResNet-18

Model ResNet-18 được xây dựng trên cấu trúc Block
![block](https://www.bing.com/images/search?view=detailV2&ccid=omYPX4m2&id=A3A858A29ADC3B1AD84111F2297B2DBF42A692A2&thid=OIP.omYPX4m2vpc13C6Nws0N9wHaFk&mediaurl=https%3a%2f%2fwww.researchgate.net%2fpublication%2f352054245%2ffigure%2ffig2%2fAS%3a1030091563859968%401622604375430%2fBasic-ResNet-Block-without-and-with-1x1-convolution.ppm&cdnurl=https%3a%2f%2fth.bing.com%2fth%2fid%2fR.a2660f5f89b6be9735dc2e8dc2cd0df7%3frik%3dopKmQr8teynyEQ%26pid%3dImgRaw%26r%3d0&exph=639&expw=850&q=block+res+net&simid=608040852969910847&FORM=IRPRST&ck=F41E7F1AB5974D93FD08BCCD56AC065B&selectedIndex=0&itb=0&ajaxhist=0&ajaxserp=0)

Sử dụng model kết hợp CrossEntropy và SGD(lr = 0.01, momentum = 0.9) cho ra kết quả chưa được tốt. Model hội tụ sau 12 epochs:
Train Loss: 0.773, Train Acc: 0.74, Valid Loss: 0.930, Valid Acc: 0.70
[loss_fig](./loss_plot.png)
[acc_fig](./acc_plot.png)
