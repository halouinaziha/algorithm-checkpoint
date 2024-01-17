# checkpoint.algo
VAR
C : CHAR:= '';
nb_char :INTEGER := 0;
nb_word :INTEGER :=1;
nb_vow :INTEGER :=0;
BEGIN
WHILE (C <> '.') DO
Read(C)
nb_char :=nb_char +1;
IF (C = 'a' OR C ='i' OR C = 'e' OR C ='o' or C = 'u' OR C ='y') then   
nb_vow := nb_vow +1;
END_IF

IF (C =' ')then
nb_vow := nb_vow +1;
END_IF

END_WHILE
Write("the length of the sentence is ",nb_char);
Write("the number of words in the sentence is",nb_word);
Write("the number of vowels in the sentence is",nb_vow);
END
