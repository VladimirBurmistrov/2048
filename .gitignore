#include <iostream>
#include <cstdlib>

int main ()
{
	std::cout << "Enter matrix 4x4. Enter numbers 2,4,8,16... plus space. Every new string begin with Enter. Good Game!\n";
	
	int matrix[4][4], i, j, m=0;
	char op;
	
	for ( i = 0; i < 4; i++) {
		for ( j = 0; j < 4; j++) {
			std::cin >> matrix[i][j];
		}
		std::cin.get(op);
	}
	
	std::cout << std::endl << "Press Enter" << std::endl;
	std::cin.get(op);
	
	for ( i = 0; i < 4; i++) {
		for ( j = 0; j < 4; j++) {
			if (matrix[i][j] == 0){
				std::cout << "* ";
			}
			else {
				std::cout << matrix[i][j] << ' ';
			}
		}
		std::cout << std::endl;
	}
	
	std::cout << "Press your letter: ";
	
	std::cin >> op;
	
	while(op == 'j' || op == 'k' || op == 'h' || op == 'l') {
		
		std::cout << std::endl;
		
		switch (op)
		{
			case 'j': 
			{
				for (j=0; j<4; j++) {
					for (i=3; i>0; i--)
					if (matrix[i] [j] == 0) {
						for (int k=i-1; k>=0; k--){
							if (matrix[k][j] != 0){
								matrix[i][j] = matrix[k][j];
								matrix[k][j]=0;
								break;
							}
						}
					}
					
				}
				
				for (j=0; j<4; j++) {
					
					for (i=3; i>0; i--){
						if (matrix[i][j] == matrix[i-1] [j]) {
							matrix[i][j] += matrix[i-1][j];
							matrix[i-1][j]=0;
							m+=matrix[i][j];
						}
					}
				}
				
				for (j=0; j<4; j++) {
					for (i=3; i>0; i--)
					if (matrix[i] [j] == 0) {
						for (int k=i-1; k>=0; k--){
							if (matrix[k][j] != 0){
								matrix[i][j] = matrix[k][j];
								matrix[k][j]=0;
								break;
							}
						}
					}
					
				}
				
				for ( i = 0; i < 4; i++) {
					for ( j = 0; j < 4; j++) {
						if (matrix[i][j] == 0){
						std::cout << "* ";
					}
					else {
						std::cout << matrix[i][j] << ' ';
					}
					}
					std::cout << std::endl;
				}
				
				std::cout << "Your goals are: " << m << std::endl << "Press your letter: ";
				
				std::cin >> op;
			
				break;
			}
		
			case 'k': 
			{
				for (j=0; j<4; j++) {
					for (i=0; i<3; i++)
					if (matrix[i] [j] == 0) {
						for (int k=i+1; k<=3; k++){
							if (matrix[k][j] != 0){
								matrix[i][j] = matrix[k][j];
								matrix[k][j]=0;
								break;
							}
						}
					}
				}
				
				for (j=0; j<4; j++) {
					for (i=0; i<3; i++)
					if (matrix[i][j] == matrix[i+1] [j]) {
						matrix[i][j] += matrix[i+1][j];
						matrix[i+1][j]=0;
						m+=matrix[i][j];
					}
				}
				
				for (j=0; j<4; j++) {
					for (i=0; i<3; i++)
					if (matrix[i] [j] == 0) {
						for (int k=i+1; k<=3; k++){
							if (matrix[k][j] != 0){
								matrix[i][j] = matrix[k][j];
								matrix[k][j]=0;
								break;
							}
						}
					}
				}
				
				for ( i = 0; i < 4; i++) {
					for ( j = 0; j < 4; j++) {
						if (matrix[i][j] == 0){
						std::cout << "* ";
					}
					else {
						std::cout << matrix[i][j] << ' ';
					}
					}
					std::cout << std::endl;
				}
				
				std::cout << "Your goals are: " << m << std::endl << "Press your letter: ";
				
				std::cin >> op;
							
				break;
			}
			
			case 'h': 
			{
				for (i=0; i<4; i++) {
					for (j=0; j<3; j++)
					if (matrix[i] [j] == 0) {
						for (int k=j+1; k<=3; k++){
							if (matrix[i][k] != 0){
								matrix[i][j] = matrix[i][k];
								matrix[i][k]=0;
								break;
							}
						}
					}
				}
				
				for (i=0; i<4; i++) {
					for (j=0; j<3; j++)
					if (matrix[i][j] == matrix[i] [j+1]) {
						matrix[i][j] += matrix[i][j+1];
						matrix[i][j+1]=0;
						m+=matrix[i][j];
					}
				}
			
				for (i=0; i<4; i++) {
					for (j=0; j<3; j++)
					if (matrix[i] [j] == 0) {
						for (int k=j+1; k<=3; k++){
							if (matrix[i][k] != 0){
								matrix[i][j] = matrix[i][k];
								matrix[i][k]=0;
								break;
							}
						}
					}
				}
			
				for ( i = 0; i < 4; i++) {
					for ( j = 0; j < 4; j++) {
						if (matrix[i][j] == 0){
						std::cout << "* ";
					}
					else {
						std::cout << matrix[i][j] << ' ';
					}
					}
					std::cout << std::endl;
				}	
				
				std::cout << "Your goals are: " << m << std::endl << "Press your letter: ";
				
				std::cin >> op;
						
				break;
			}
			
			case 'l': 
			{
				for (i=0; i<4; i++) {
					for (j=3; j>0; j--)
					if (matrix[i] [j] == 0) {
						for (int k=j-1; k>=0; k--){
							if (matrix[i][k] != 0){
								matrix[i][j] = matrix[i][k];
								matrix[i][k]=0;
								break;
							}
						}
					}
				}
				
				for (i=0; i<4; i++) {
					for (j=3; j>0; j--)
					if (matrix[i][j] == matrix[i] [j-1]) {
						matrix[i][j] += matrix[i][j-1];
						matrix[i][j-1]=0;
						m+=matrix[i][j];
					}
				}
				
				for (i=0; i<4; i++) {
					for (j=3; j>0; j--)
					if (matrix[i] [j] == 0) {
						for (int k=j-1; k>=0; k--){
							if (matrix[i][k] != 0){
								matrix[i][j] = matrix[i][k];
								matrix[i][k]=0;
								break;
							}
						}
					}
				}
				
				for ( i = 0; i < 4; i++) {
					for ( j = 0; j < 4; j++) {
						if (matrix[i][j] == 0){
						std::cout << "* ";
					}
					else {
						std::cout << matrix[i][j] << ' ';
					}
					}
					std::cout << std::endl;
				}
				
				std::cout << "Your goals are: " << m << std::endl << "Press your letter: ";
				
				std::cin >> op;
				
				break;
			}
		}
	}
	
	return 0;
}
