# flower-lingrui
> 说明1：此实验的数据集过大，就不放进仓库了，正确的数据放置方式如下
              
data/         
├── train/              
│   ├── daisy/                
│   │   └── *.jpg              
│   ├── dandelion/                
│   ├── rose/               
│   ├── sunflower/               
│   └── tulip/             
└── test/               
    ├── daisy/             
    ├── dandelion/              
    ├── rose/              
    ├── sunflower/              
    └── tulip/                 


> 说明2：程序运行时，会自动生成以下文件和文件夹，用以记录                                      
                   
logs/                          
├── bad_img        # 坏图清单（文本文件，记录每张坏图的来源路径）              
├── best.pth       # 训练过程中产生的最佳模型权重             
└── broken/        # 被检测出来、从 data 里移出来的坏图               
    └── xxx.jpg                                 
 

> 说明3：仓库文件结构如下：
                  
花卉识别/              
├── data/              
│   └── 这里放入花卉数据集                
├── docx/                 
│   ├── accuracy_curve.png                                 
│   ├── loss_curve.png                        
│   ├── 花卉题解.md               
│   └── 花卉题解.pdf                  
├── src/                     
│   ├── config.py                
│   ├── dataloader.py                    
│   ├── dataset.py                  
│   ├── main.py             
│   ├── model.py                
│   ├── plot.py              
│   ├── preprocess.py                    
│   └── train.py                                   
└── README.md                     
