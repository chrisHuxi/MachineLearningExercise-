# Machine Learning Exercise

exercise of ML course in TUD, [exercise description and sildes click here](http://cvl.inf.tu-dresden.de/courses/machine-learning-1/).

## week4 : Decision Tree with continuous value
#### including :
 * [DecisionTree_cont_var.py](https://github.com/chrisHuxi/MachineLearningExercise/blob/master/week4_decision_tree_cont_variables/DecisionTree_cont_var.py)
 * [DT_skt.py](https://github.com/chrisHuxi/MachineLearningExercise/blob/master/week4_decision_tree_cont_variables/DT_skt.py)
 * [DT_gain_ratio.py](https://github.com/chrisHuxi/MachineLearningExercise/blob/master/week4_decision_tree_cont_variables/DT_gain_ratio.py)
 * [data](https://github.com/chrisHuxi/MachineLearningExercise/tree/master/week4_decision_tree_cont_variables/data)
### The result as following : 

* P1 DecisionTree_cont_var : my implementation:


![](https://github.com/chrisHuxi/MachineLearningExercise/blob/master/week4_decision_tree_cont_variables/result/P1.PNG)


* P2 DecisionTree : scikit-learn implementation:


![](https://github.com/chrisHuxi/MachineLearningExercise/blob/master/week4_decision_tree_cont_variables/result/P2.PNG)


* P3 DecisionTree : with gain ratio, on the "Data3.csv":


![](https://github.com/chrisHuxi/MachineLearningExercise/blob/master/week4_decision_tree_cont_variables/result/P3.PNG)




## week3 : Decision Tree
### edit:
 * I took a mistake : in my original code, every time I produce a node I set a feature as "false", so that the final decision tree is small and with lower accuracy. 
 * so we should change code in `dtree_learning(examples, attr_avail, default, cls_index)` in line 133. As follow:
  ```python
     #attr_avail[best_attr_index] = False # original code
     new_attr_avail = attr_avail[:best_attr_index]+[False]+attr_avail[best_attr_index+1:]   #edited code
  ```
 * result of new code : 
 
    ![](https://github.com/chrisHuxi/MachineLearningExercise/blob/master/week3_decision_tree/result_dt_plus.PNG)
   
 * [edited code click here](https://github.com/chrisHuxi/MachineLearningExercise/blob/master/week3_decision_tree/DecisionTree_plus.py)
 * reference : [code from Professor Guthier](http://cvl.inf.tu-dresden.de/HTML/teaching/courses/ml1/ss18/Ex/3/tree.py)

### including :
 * [DecisionTree.py](https://github.com/chrisHuxi/MachineLearningExercise/blob/master/week3_decision_tree/DecisionTree.py)
 * [data set](https://github.com/chrisHuxi/MachineLearningExercise/tree/master/week3_decision_tree/data)

### The result as following : 

![](https://github.com/chrisHuxi/MachineLearningExercise/blob/master/week3_decision_tree/result_dt.PNG)



## week2 : visualize
### including :
 * [2D_gaussian_distribution.py](https://github.com/chrisHuxi/MachineLearningExercise/blob/master/week2_visualize/2D_gaussian_distribution.py)
 * [visualize.py](https://github.com/chrisHuxi/MachineLearningExercise/blob/master/week2_visualize/visualize.py)
 * [data : DatAccel.txt](https://github.com/chrisHuxi/MachineLearningExercise/blob/master/week2_visualize/DatAccel.txt) , [data : DatGyr.txt](https://github.com/chrisHuxi/MachineLearningExercise/blob/master/week2_visualize/DatGyr.txt)
 
### The result as following : 

* P1 gaussian distribution:


  ![](https://github.com/chrisHuxi/MachineLearningExercise/blob/master/week2_visualize/P1_result.png)


* [covariance matrix, which calculated from generated data : ](https://github.com/chrisHuxi/MachineLearningExercise/blob/master/week2_visualize/P1_result.txt)

* P2 visualize : 


  ![](https://github.com/chrisHuxi/MachineLearningExercise/blob/master/week2_visualize/P2_result_1.png)
