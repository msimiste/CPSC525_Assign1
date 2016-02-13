

#include <stdio.h>

main()
{
unsigned char buffer[] = "\xa0";

	FILE *write_ptr;
	write_ptr = fopen("file1.bin","wb");  // w for write, b for binary
	fwrite(buffer,1, sizeof(buffer),write_ptr); // write 10 bytes to our buffer
	fclose(write_ptr);
	write_ptr = fopen("file2.bin", "wb");
	unsigned char buffer1[] = "\x2a\xef                              ";
	fwrite(buffer1,1, sizeof(buffer1), write_ptr);
	fclose(write_ptr); 
	write_ptr = fopen("file3.bin", "wb");
	unsigned char buffer2[] = "\x33\x33\x33\x33\x33\x33\x33\x33\x33\x33\x33\x33\x33\x33\x33\x33\x33\x33\x33\x33\x33\x33\x33\x33\x33\x33\x33\x33\x33\x33\x33\x33\x55\x55\x55\x55\x44\x44\x44\x44";
	fwrite(buffer2, 1, sizeof(buffer2), write_ptr);
	fclose(write_ptr);
	
	write_ptr = fopen("file4.bin", "wb");
	unsigned char buffer3[] = "\x99\x99\x99\x99\x99\x99\x99\x99\x99\x99\x99\x99\x99\x99\x99\x99\x99\x99\x99\x99\x99\x99\x99\x99\xad\x88\x04\x08";
	fwrite(buffer3, 1, sizeof(buffer3), write_ptr);
	fclose(write_ptr);

	return 0;

}

