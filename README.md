# DoCompiler
Programming Language &amp; Compiler

## Phase 1 — Lexer
```
let x = 10;
```
→
```
LET
IDENTIFIER(x)
EQUAL
NUMBER(10)
SEMICOLON
```

## Phase 2 — Parser
Tạo AST:
```
      Assignment
       /       \
      x         10
```

## Phase 3 — Semantic Analysis
Kiểm tra:
```
x = 10
x + "hello"
```
phát hiện:
```
Type Error
```

## Phase 4 — Interpreter
Ban đầu:
```
Nova Source
     ↓
AST
     ↓
Interpreter
```
Chưa cần machine code.

## Phase 5 — Bytecode VM
Chuyển:
```
Nova
 ↓
Bytecode
 ↓
Nova VM
```

## Phase 6 — Compiler Optimization
Nghiên cứu:
```
Constant Folding

Dead Code Elimination

Common Subexpression Elimination

Loop Optimization

Inlining

Register Allocation
```

## Phase 7 — Native Code
Cuối cùng:
```
Nova
 ↓
IR
 ↓
Machine Code
```
Có thể target:
```
x86-64
ARM64
RISC-V
```
Nếu muốn nghiên cứu sâu:
| RISC-V
