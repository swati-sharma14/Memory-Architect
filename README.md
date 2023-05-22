# Memory Architect 	🧠

This program helps users understand and visualize the organization of memory within a computer system. It provides information about different types of memory and allows users to solve various memory-related questions.

## Types of Memory 📚

1. Bit Addressable Memory - Cell Size = 1 bit
2. Nibble Addressable Memory - Cell Size = 4 bits
3. Byte Addressable Memory - Cell Size = 8 bits (standard)
4. Word Addressable Memory - Cell Size = Word Size (depends on CPU)

Note: Byte Addressable Memory is the industry standard unless otherwise mentioned.

Important Note: CPUs are always word addressable, which means the number of bits in a CPU represents its word size. An interface is required to connect the CPU with memory.

## Memory Architect CLI 💻

The Memory Architect CLI is a command-line program that allows users to input information and interact with the memory-related features.

### Queries ❓

The program supports processing different types of memory-related queries:

1. Instruction Set Architecture (ISA) and Instructions:
   - Type A Query: `<Q bit opcode> <P-bit address> <7 bit register>`
   - Type B Query: `<Q bit opcode> <R bits filler> <7 bit register> <7 bit register>`

For each type of query, the following information should be provided as input:

- Length of one instruction in bits
- Length of a register in bits

The program will output the following information:

- Minimum number of bits needed to represent an address in this architecture
- Number of bits needed for the opcode
- Number of filler bits in Type B instruction
- Maximum number of instructions supported by this ISA
- Maximum number of registers supported by this ISA

2. System Enhancement Queries:
   - Type 1 Query:
     - Number of bits in the CPU
     - Desired change in the current addressable memory to any of the three remaining options

   Output:
   - Number of address pins saved or required (indicated by "-" for saved pins and "+" for additional pins)
   - Note: The memory size and current addressability are carried over from the initial inputs.

   - Type 2 Query:
     - Number of bits in the CPU
     - Number of address pins available in the CPU
     - Type of addressable memory (choose one of the four options)

   Output:
   - Maximum size of the main memory in bytes (excluding the initial inputs of addressability and memory space)

## Examples 🌟

To understand the input format and how the program works, refer to the provided examples. They cover different types of queries and provide the expected output.

Feel free to explore and use the Memory Architect program to gain insights into memory organization. If you encounter any issues or have suggestions for improvement, please don't hesitate to open an issue or submit a pull request.
