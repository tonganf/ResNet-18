## ResNet-18

Model ResNet-18 được xây dựng trên cấu trúc Block

<div align="center">
  <img src="https://www.researchgate.net/publication/352054245/figure/fig2/AS:1030091563859968@1622604375430/Basic-ResNet-Block-without-and-with-1x1-convolution.ppm" width="50%" height="250"><br><br>
</div>

Sử dụng model kết hợp CrossEntropy và SGD(lr = 0.01, momentum = 0.9) cho ra kết quả chưa được tốt. Model hội tụ sau 12 epochs:
Train Loss: 0.773, Train Acc: 0.74, Valid Loss: 0.930, Valid Acc: 0.70

<div align="center">
    <img src='./loss_plot.png' width="70%" height = '60%'>
</div>

**Loss** trên cả tập `train` và `test` đều hội tụ nhanh sau epoch 10. Từ epoch 10 loss trên tập `valid` bắt đầu đi ngang nhưng trên tập `train` vẫn tiếp tục giảm.

<div align="center">
    <img src='././acc_plot.png' width="70%" height = '60%'>
</div>
Độ chính xác của mô hình trên tập `train` chưa được cao (0.8) và ở tập `valid`(0.7). Có độ chênh lệch lớn `accuracy` trên 2 tập `train` và `valid`.(Model vẫn chưa khái quát được dữ liệu chưa nhìn thấy - high variance)
