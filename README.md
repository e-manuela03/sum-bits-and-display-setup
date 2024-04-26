# sum-bits-and-display-setup
Display the sum of the inputs signals or which one is bigger on xc7s50csga324-1 8 led display


The circuit receives two 2-bit numbers, a and b, and two independent selection bits, sel_op and show_sum. If sel_op is 0, the highest bit sum is chosen, so the output of MUX_COMP will provide 1 if the bit sum of a is greater than the bit sum of b, and vice versa. If sel_op is 0, the lowest sum of bits is chosen, so the output of MUX_COMP will provide 1 if the sum of bits of a is less than the sum of bits of b and vice versa. If show_sum is 0, TOP will output the 7-bit encoded input that has the higher/lower bit sum depending on the sel_op selection bit chosen. If show_sum is 1, TOP will provide its output with the bit sum of the corresponding input (which has the lower/higher bit sum depending on sel_op).

