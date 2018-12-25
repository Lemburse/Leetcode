class Solution:
    def isValidSudoku(self, board):
        """
        :type board: List[List[str]]
        :rtype: bool
        """
        
        for i in range(9):
            v = []
            for p in board[i]:
                if p!='.':
                    v.append(p)
            if len(v) !=len(set(v)):
                return False
            else:
                v = []
            #行向量结束
            u = []
            for j in range(9):
                for q in board[j][i]:
                    if q != ".":
                        u.append(q)
            if len(u) != len(set(u)):
                    return False
            else:
                u =[]
            #列向量结束
        w =[]
        for k in [0,3,6]:
            for l in [0,3,6]:
                for x in range(k,k+3):
                    for y in range(l,l+3):
                            if board[x][y] != ".":
                                w.append(board[x][y])
                if len(w) != len(set(w)):
                    return False
                else:
                    w = []
        return True
