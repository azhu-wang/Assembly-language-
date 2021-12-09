PrintStr	macro string                                           		 ;print string
            lea dx,string
            mov ah,09h
            int 21h
            endm			
Sort	macro  SortData, i 
        mov  bx,0h    
		mov  dx,0h		
		mov  cx,i 
		push cx
		dec  cx
		L1:
			cmp cx,0                                 					 ;bubble sorting
			je  Pout
			mov dl,SortData[bx]
			cmp dl,SortData[bx+1]
			jb  Exchange                                                 ;make the biggest number in the left
			inc bx
			cmp bx,cx                                                    ;if it's first run ending,turn to L2 make the second run
			je  L2
			jmp L1		
		L2:
			mov bx,0                                                     ;fix the biggest number,so cx -1
			dec cx
			jmp L1
		Exchange:     		                         					 ;exchange the number
			mov al,SortData[bx+1]
			mov SortData[bx],al
			mov SortData[bx+1],dl
			jmp L1
		Pout:  
			pop cx		                                                 ;pop the cx befores
			mov bx,0h
		P1:	
			mov dl,SortData[bx]
			inc bx
			add dl,30h
			cmp dl,3Ah                             					     ;ASCII's difference, so +30h or +37h
			jb  P2
			add dl,07h                                  
		P2:	
			mov ah,02h                               				     ;print
			int 21h
			loop P1
			endm		
.8086
.model small
.stack 1024
.data
str1     db  "===========hw2===========",10,13,"Sorting result:$"   		 ;the string we wanna print
str2     db  10,13,"=========================$"
SortData db  08h,01h,0ah,0ch,04h,05h,06h,'$'                            		 ;our data
i        dw  7
.code
.startup
	PrintStr str1                                                   	;main function
	Sort 	 SortData, i
	PrintStr str2
.exit
end
