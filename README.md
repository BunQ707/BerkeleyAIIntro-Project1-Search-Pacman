# BerkeleyAIIntro-Project1-Search-Pacman

Bài tập AI

Bài 1+2: DFS + BFS
  Mục tiêu của bài này là tạo một vòng lặp while để duyệt qua các state theo dfs hoặc bfs:
   - Pop một state ra 
   - Gọi hàm getSuccessors để tìm kiếm lần lượt các state tiếp theo
   - Lặp lại
  Output là một list các action dẫn đến goal, ta gắn list đó với mỗi state, tức là mỗi state có một path từ state đầu đến state đó.
  Để cho tiện, ta tạo cho mỗi phần tử trong stack/queue một cấu trúc: ( state, path )
  VD: stack.pop ( startState, [] )
  
  Dễ thấy mỗi lần gọi hàm getSuccessors thì nó còn trả về ( state, action, cost ) nên path của state đó là prevState.path +action .
  Như vậy nếu ta xác định được một state là goal thì ta cũng return được path đến nó.
  
  
