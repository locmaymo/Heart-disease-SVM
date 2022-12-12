# Hi
## Tạo biểu đồ trên grafana từ mysql trên máy
![image](https://user-images.githubusercontent.com/52437817/206948560-8fcff531-e739-441d-8589-8757b4b6fe1e.png)
### query pannel SVM tự thiết lập : 
SELECT * FROM
(SELECT COUNT(*) as correct FROM btl_iot.accuracy_tbl where actual = predict) as correct,
(SELECT COUNT(*) as incorrect FROM btl_iot.accuracy_tbl where actual <> predict) as incorrect;
