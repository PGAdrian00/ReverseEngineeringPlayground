# AssemblerPlayground
Learning the use of asm through exercise and working my way to be able to understand reverse engeneering part 1.
  In rec.asm I go through the basic hello world type exercise and a basic(not so intuitive) for loop :)
  In math.asm I implement functions using proc and endp and define arrays of numbers to go through and find different things:
    a -> find the prime numbers
    b -> find the sum of numbers that are multiple of 5
    c -> find the 2 biggest numbers in that array
    (d) implement and experience how to use cdecl (cdeclaration way of writing), stdcall(standard call), fastcall.
    cdecl -> caller frees stack, parameters are pushed in reverse order and the return value is in EAX. (default for C/C++ functions), usefull for function whose nr of args we don t know.
    stdcall -> callee is responsible for cleaning of the stack, parameters are pushed in reverse order, returns in EAX, stack is balanced being cleaned by callee. Usefull for windowsAPI
    fastcall -> puts some of the arguments directly in registers (ECX EDX), callee cleans stack, way faster and returns in EAX.
