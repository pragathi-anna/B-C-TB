module fourbit (a,b,cin,s,cout);
input logic [3:0] a;      
input logic [3:0] b;   
input logic cin;   
output logic [3:0] s; 
output logic cout ; 
logic [4:0] sum; 
assign sum = a + b + cin;
assign s = (sum > 9) ? (sum + 6) :sum[3:0];
assign cout = (sum > 9);
endmodule


module eightbit(a,b,cin,s,cout);
input logic[7:0] a,b;
input logic cin;
output logic[7:0] s;
output logic cout;
logic[3:0] s1,s2;
logic c1,c2;
fourbit I1 (a[3:0],b[3:0],cin,s1,c1);
fourbit I2 (a[7:4],b[7:4],c1,s2,c2);
assign s={s2,s1};
assign cout=c2;
endmodule
