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
		
		-混淆矩陣
			metrics.confusion_matrix
  	
  
  -
