NAME = matrix.a	
SRC = ./srcs/matrix.c
INC = ./includes/	
OBJ= $(SRC:.c=.o)
CC = gcc	
FLAGS= -Wall -Werror -Wextra 	
PARA  = -c	

%.o: %.c
	$(CC) $(PARA) -I $(INC) $(FLAGS) -o $@ $<

all: $(NAME)	

$(NAME): $(OBJ)		
	ar rc $(NAME) $(OBJ)	

clean:	
	rm -f $(OBJ)	

fclean: clean	
	rm -f $(NAME)	
	rm -f includes/*.*.gch	

re: fclean all