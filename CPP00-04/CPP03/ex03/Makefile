# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: emsoares <emsoares@student.42porto.com>    +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2023/11/08 14:35:14 by emsoares          #+#    #+#              #
#    Updated: 2023/11/08 14:35:14 by emsoares         ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

RESET   = \033[0m
BLACK   = \033[1;30m
RED     = \033[1;31m
GREEN   = \033[1;32m
YELLOW  = \033[1;33m
BLUE    = \033[1;34m
PURPLE  = \033[1;35m
CYAN    = \033[1;36m
WHITE   = \033[1;37m

NAME = ex03

CXX = c++

CXXFLAGS = -Wall -Wextra -Werror -std=c++98

RM = rm -rf

SRCS = main.cpp \
	ClapTrap.cpp \
	ScavTrap.cpp \
	FragTrap.cpp \
	DiamondTrap.cpp \

OBJS = $(SRCS:%.cpp=%.o)

all: $(NAME)

$(NAME): $(OBJS)
	@$(CXX) $(CXXFLAGS) $(OBJS) -o $(NAME)
	clear
	@echo "$(GREEN)./ex03 executable is ready!$(RESET)"

clean:
	@$(RM) $(OBJS)
	@echo "$(RED)Object files have been deleted!$(RESET)"

fclean: clean
	@$(RM) $(NAME) 
	clear
	@echo "$(RED)Object and Executable files have been deleted!$(RESET)"

re: fclean all