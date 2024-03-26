# ResNet-18

Model ResNet-18 được xây dựng trên cấu trúc Block

<div align="center">
  <img src="./ResNet18/Block_Resnet.png" width="50%" height="250"><br><br>
</div>

Sử dụng model kết hợp CrossEntropy và SGD(lr = 0.01, momentum = 0.9) cho ra kết quả chưa được tốt. Model hội tụ sau 12 epochs:
Train Loss: 0.773, Train Acc: 0.74, Valid Loss: 0.930, Valid Acc: 0.70

<div align="center">
    <img src='./ResNet18/loss_plot.png' width="60%" height = '50%'>
</div>

**Loss** trên cả tập `train` và `test` đều hội tụ nhanh sau epoch 10. Từ epoch 10 loss trên tập `valid` bắt đầu đi ngang nhưng trên tập `train` vẫn tiếp tục giảm.

<div align="center">
    <img src='./ResNet18/acc_plot.png' width="60%" height = '50%'>
</div>
Độ chính xác của mô hình trên tập `train` chưa được cao (0.8) và ở tập `valid`(0.7). Có độ chênh lệch lớn `accuracy` trên 2 tập `train` và `valid`.(Model vẫn chưa khái quát được dữ liệu chưa nhìn thấy - high variance)

## Regularization

Mô hình khi kết hợp với regularization - SGD(lr=0.001, weight_decay=5e-4) ở epoch thứ 10 mặc dù lr thấp hơn rất nhiều nhưng hội tụ nhanh.

<div align="center">
    <img src='./ResNet18/acc_plot_reg_lr0.001.png' width="60%" height = '50%'>
</div>

Mô hình hội tụ nhanh hơn và độ chênh lệch giữa `trainset` và `validset` nhỏ hơn đáng kể `(giảm được variance)`

<div align="center">
    <img src='./ResNet18/loss_plot_reg_lr0.001.png' width="60%" height = '50%'>
</div>
=======
# ResNet-18

