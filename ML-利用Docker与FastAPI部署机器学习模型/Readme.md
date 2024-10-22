首先利用机器学习预测混凝土抗压强度并进行模型持久化，然后基于Docker与FastAPI形成API应用，接口已经通过postman测试。数据来源：[https://www.kaggle.com/datasets/sinamhd9/concrete-comprehensive-strength](https://www.kaggle.com/datasets/sinamhd9/concrete-comprehensive-strength)

.ML-利用Docker与FastAPI部署机器学习模型
├── Appendix-files
│   ├── Readme.md
│   └── figures
│       ├── Postman_result.png
│       ├── containerize-app1.png
│       └── model-deployment.png
├── Dockerfile
├── ML-利用Docker与FastAPI部署机器学习模型.ipynb
├── Readme.md
├── app
│   ├── __init__.py
│   └── main.py
├── model
│   └── RF_model.pkl
└── requirements.txt
