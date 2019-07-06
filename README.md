# chessboad
import numpy as np
chessBoard=np.zeros((8,8),dtype=int)

#print(chessBoard)

chessBoard[1::2,::2]=1
chessBoard[::2,1::2]=1



queenPosition1=input("where to place 1st queen: ")
queenPosition2=input("where to place 2nd queen: ")
queenPosition3=input("where to place 3rd queen: ")
queenPosition4=input("where to place 4th queen: ")

q1=queenPosition1.split(',')
q2=queenPosition2.split(',')
q3=queenPosition3.split(',')
q4=queenPosition4.split(',')

chessBoard[int(q1[0])][int(q1[1])] =9
chessBoard[int(q2[0])][int(q2[1])] =9
chessBoard[int(q3[0])][int(q3[1])] =9
chessBoard[int(q4[0])][int(q4[1])] =9


"""
print(queenPosition1,type(queenPosition1))
print(queenPosition2,type(queenPosition2))
print(queenPosition3,type(queenPosition3))
print(queenPosition4,type(queenPosition4))
"""
print(chessBoard,chessBoard.shape,chessBoard.ndim)
