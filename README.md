COMPANY: CODTECH IT SOLUTIONS

NAME: SYED TAUSEEF ASHRAF

INTERN ID: COMPANY: CT06DF1544

DOMAIN: VLSI

DURATION: 6 WEEKS

MENTOR: NEELA SANTOSH

** In task 3, the goal was to project and simulate a 4 -stage piping processor using Verilog HDL. The processor was designed to perform basic operations such as Add, Sub and Load. The entire architecture was structured in four main steps of pipeline: Instruction Search (SE), instruction decoding (ID), executing (ex) and writing back (WB). Each of these stages has been implemented to allow parallelism at the level of instruction, where several instructions are processed simultaneously, but at different stages of the pipeline, thus improving the general execution transfer rate. The pipeline structure is a fundamental concept in computer architecture that helps increase performance, overlapping the execution of instruction.

To test the processor, a simple testBench Verilog was created. The pipeline_processor module was instantiated inside the TestBench module called pipeline_tab_tb. TestBench was responsible for generating clock and redefinition signals, memory value boot and records, and controlling simulation time. A watch signal was alternated using a loop forever with a fixed time interval, and the redefinition signal was initially stated and then awakened after a small delay to start normal execution. A basic instruction like Addi (Add immediately) has been manually charged in instruction memory and corresponding origin records have been initialized. This configuration allowed the correct search for operating, execution and result writing in the appropriate stages of pipeline.

The simulation was performed using the EDA playground platform. Signal transitions were recorded using Verilog's $ dumpfile and $ dumpvars tasks, and waveforms were analyzed through the EPWAE viewer. The waveform displayed a clear view of how the instruction progressed through each pipeline stage. Internal signals such as instruction_id, opcode_id, operand1_id, operand2_ex, rd_ex and result_wb were observed. The transitions of these signs corresponded to the expected values, confirming the correct behavior of the pipeline. During the simulation, initial indefinite states (X) were observed for some signs, which is normal before the redefinition was released. After redefinition, all values stabilized and the signs reflected the flow of instructions expected through the watch cycles.

Design ensures that each instruction takes a cycle per internship and that various instructions can occupy different stages at once. The wave form output clearly illustrated this pipeline behavior, showing various active instructions in the IF, ID, EX and WB stages during overlapping cycles. Watch and redefinition signals were also captured as wave, confirming the proper synchronous operation. The successful backback of the registration file result has confirmed the processor's ability to execute the state-to-end instruction.

This task provided a deeper understanding of the pipeline processor design and its practical challenges. It helped strengthen the skills in Verilog coding, signal tracking, test creation and clearance using wave shape simulations. Through this implementation, the fundamental concepts of pipelining, such as data movement between internships, instructions overlap and execution time, were clearly demonstrated. The processor can be extended even more in the future to deal with more complex operations,
