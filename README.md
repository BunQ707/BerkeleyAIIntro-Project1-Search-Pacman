# BerkeleyAIIntro-Project1-Search-Pacman

Bài tập AI

Bài 1+2: DFS + BFS
  Solution giống nhau chỉ khác cấu trúc dữ liệu, stack hay queue, do vậy viết một solution chung.
  Pop ra một state, dò các state tiêp theo rồi cho vào cấu trúc, cứ thế đến khi cấu trúc là empty hoặc đã phát hiện ra goal.
  
Bài 3: UCS
  Giống bài trên nhưng dùng priority queue, dùng class được cung cấp sẵn: PriorityQueueWithFunction(cost) với chi phí cost = problem.getCostOfActions (có sẵn)
  
Bài 4:
  Giống bài 3 nhưng bây giờ cost = f(x) = g(x) + h(x) với 2 hàm/method được cung cấp sẵn:
  g(x) = problem.getCostOfActions 
  h(x) = heuristic(state, problem) (như trong đề bài thì đó là khoảng cách manhattan)
  
Bài 5:
  Một state gồm vị trí của nó state[0] và vị trí các góc state[1]
  Chỉ cần sửa lại 3 method: getStartState trả về vị trí bắt đầu và list các góc; isGoalState trả về đã hết góc chưa (dùng len state[1] ); getSuccessors dò 4 hướng để lấy state   tiếp theo liền kề, bỏ tường, lưu ý loại bỏ nó khỏi list góc nếu chính nó là góc.
  
Bài 6:
  Tiếp tục bài 5, cài đặt một thuật toán đánh giá: tìm khoảng cách manhattan đến mỗi góc rồi lấy lớn nhất.

  
