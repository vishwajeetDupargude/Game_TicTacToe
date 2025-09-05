# Game_TicTacToe
import numpy as np
import random
from time import sleep


def create_board():
    return np.zeros((3,3), dtype=int)

def possablites(board):
    return [(i,j)
    for i in range(3):
        for j in range(3)
    if board[i][j]==0]


def random_place(board,player):
    loc= random.choice(possablites(board))
    board[loc]= player
    return board

def win_ratio()    
