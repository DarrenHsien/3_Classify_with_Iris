# 3_Classify_with_Iris
Different types of classify's method

1.KNN最鄰近分類

	-KNeighborsClassifier

		-n_neighbors : 根據最近多少個鄰居K來決定類別

		-weights : 

			-uniform : 最近k個鄰居的權重一樣來決定類別

			-distance : 最近k個鄰居的權重根據距離成反比決定類別
  
	-RadiusNeighborsClassifier
    
		-radius : 根據最近多少個鄰居K來決定類別

		-weights : 

			-uniform : 根據方圓距離內鄰居來決定類別

			-distance : 根據方圓距離內鄰居根據距離成反比決定類別


  	-評估準確度
  		
		-準確度
			metrics.classification_report
				
				-Precision
				
				-recall
				
				-f1-score
		
		-混淆矩陣
			metrics.confusion_matrix
  				
2.SVM支持向量機
	
	目標 : 求取可拆分資料的最大邊界(超平面)
	
	權重係數即為描述邊界的相關係數
	
	Kernel(C) : 排除資料線性不可分問題
	
	-SVC(C=1.0, kernel="rbf")
		
		-C : 根據錯誤分類的懲罰，C越大切割線就會切得更複查
		
		KERNAL : 
		
			-rbf : 用來處理非線性的切割線
			
			-linear : 線性(如果使用此kernel可直接使用LinearSVC不需要使svc
			
			-poly 
	
	-評估準確度
  		
		-準確度
			metrics.classification_report
				
				-Precision
				
				-recall
				
				-f1-score
		
		-混淆矩陣
			metrics.confusion_matrix
  	
	
	
	
	
	
