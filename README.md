# kubernete-cross-ns

1.先建立另一個namespace
2.把mysql指定建立在新的namespace下
3.App的連線資訊設定在application.yml裡，修改mapping mysql的name，格式為<Service Name>.<Namespace Name>
4.重新build image並打包至docker hub(新版號)

另外給App開了NodePort，讓外部可使用NodePort連App Web而不用再手動開proxy
