# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: ryoshio- <ryoshio-@student.42sp.org.br     +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2023/05/26 22:02:27 by ryoshio-          #+#    #+#              #
#    Updated: 2023/07/06 23:08:18 by ryoshio-         ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

NAME = ex04

CC = c++

CFLAG = -Wall -Wextra -Werror -std=c++98

SRC = main.cpp Check.cpp Replace.cpp

VALGRIND = valgrind 

OBJ = $(SRC:.cpp=.o)

all: $(NAME)

$(NAME): $(OBJ)
	$(CC) $(CFLAG) $(OBJ) -o $(NAME)

run: all
	$(VALGRIND) ./$(NAME)

clean:
	rm -rf $(OBJ)

fclean: clean
	rm -rf $(NAME)

re: fclean all

.PHONY: all clean fclean re 