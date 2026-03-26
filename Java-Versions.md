# Java Version Major Features

### Java 8 (LTS - March 2014)

- **Lambda Expressions:** Functional programming with concise syntax (x -> x * 2)
- **Stream API:** Functional-style operations on collections (filter, map, reduce)
- **Optional:** Container to avoid NullPointerException
- **Default Methods:** Interface methods with implementation
- **Method References:** Shorthand for lambdas (System.out::println)
- **New Date/Time API:** java.time package (LocalDate, LocalDateTime, ZonedDateTime)
- **Functional Interfaces:** @FunctionalInterface annotation
- **Nashorn JavaScript Engine:** Embedded JavaScript runtime
- **CompletableFuture:** Asynchronous programming support

### Java 9 (September 2017)

- **Module System (Project Jigsaw):** Modular JDK with module-info.java
- **JShell:** Interactive REPL for Java
- **Private Interface Methods:** Private methods in interfaces
- **Collection Factory Methods:** List.of(), Set.of(), Map.of()
- **Stream Improvements:** takeWhile(), dropWhile(), ofNullable()
- **Optional Improvements:** ifPresentOrElse(), or(), stream()
- **Process API Updates:** ProcessHandle for process management
- **HTTP/2 Client (Incubator):** Modern HTTP client
- **Multi-Release JAR Files:** Version-specific class files

### Java 10 (March 2018)

- **Local Variable Type Inference:** var keyword for local variables
- **Garbage Collector Interface:** Clean GC interface
- **Application Class-Data Sharing:** Improved startup time
- **Thread-Local Handshakes:** Per-thread callbacks
- **Optional.orElseThrow():** No-arg version throws NoSuchElementException
- **Unmodifiable Collection Improvements:** copyOf() methods

### Java 11 (LTS - September 2018)

- **HTTP Client (Standard):** java.net.http package finalized
- **Local-Variable Syntax for Lambda:** var in lambda parameters
- **String Methods:** isBlank(), lines(), strip(), repeat()
- **Files Methods:** readString(), writeString()
- **Collection to Array:** toArray(IntFunction)
- **Nest-Based Access Control:** Private member access in nested classes
- **Running Single-File Programs:** java HelloWorld.java directly
- **Epsilon GC:** No-op garbage collector
- **ZGC (Experimental):** Scalable low-latency GC

### Java 12 (March 2019)

- **Switch Expressions (Preview):** Arrow syntax, yield
- **Compact Number Formatting:** NumberFormat.getCompactNumberInstance()
- **Teeing Collector:** Collectors.teeing() for dual collection
- **String Methods:** indent(), transform()
- **Files.mismatch():** Compare file contents
- **Shenandoah GC (Experimental):** Low-pause-time GC

### Java 13 (September 2019)

- **Text Blocks (Preview):** Multi-line strings with """
- **Switch Expressions (Second Preview):** Refined syntax
- **Dynamic CDS Archives:** Easier class-data sharing
- **ZGC Improvements:** Uncommit unused memory
- **Socket API Reimplementation:** Modern implementation

### Java 14 (March 2020)

- **Switch Expressions (Standard):** Finalized feature
- **Records (Preview):** Immutable data classes
- **Pattern Matching for instanceof (Preview):** No cast needed
- **Helpful NullPointerExceptions:** Detailed NPE messages
- **Text Blocks (Second Preview):** Escape sequences
- **Foreign Memory Access API (Incubator):** Safe native memory access
- **NUMA-Aware Memory Allocation for G1**

### Java 15 (September 2020)

- **Text Blocks (Standard):** Finalized feature
- **Sealed Classes (Preview):** Restricted class hierarchies
- **Records (Second Preview):** Refined feature
- **Pattern Matching for instanceof (Second Preview)**
- **Hidden Classes:** Framework-generated classes
- **ZGC (Production Ready):** No longer experimental
- **Shenandoah GC (Production Ready)**
- **Edwards-Curve Digital Signature Algorithm (EdDSA)**

### Java 16 (March 2021)

- **Records (Standard):** Finalized feature
- **Pattern Matching for instanceof (Standard):** Finalized
- **Sealed Classes (Second Preview)**
- **Vector API (Incubator):** SIMD operations
- **Foreign Linker API (Incubator):** Native code interop
- **Stream.toList():** Efficient list collection
- **Day Period Support:** DateTimeFormatter with 'B' pattern
- **Unix-Domain Socket Channels**

### Java 17 (LTS - September 2021)

- **Sealed Classes (Standard):** Finalized feature
- **Pattern Matching for switch (Preview):** Switch on types
- **Foreign Function & Memory API (Incubator):** Replace JNI
- **Vector API (Second Incubator)**
- **Context-Specific Deserialization Filters**
- **Enhanced Pseudo-Random Number Generators**
- **Deprecate Applet API for Removal**
- **Strong Encapsulation of JDK Internals by Default**
- **macOS/AArch64 Port:** Apple Silicon support

### Java 18 (March 2022)

- **Simple Web Server:** jwebserver command for static files
- **Code Snippets in Javadoc:** @snippet tag
- **UTF-8 by Default:** Standard charset
- **Vector API (Third Incubator)**
- **Foreign Function & Memory API (Second Incubator)**
- **Pattern Matching for switch (Second Preview)**
- **Deprecate Finalization for Removal**

### Java 19 (September 2022)

- **Virtual Threads (Preview - Project Loom):** Lightweight threads
- **Structured Concurrency (Incubator):** Concurrent task management
- **Record Patterns (Preview):** Deconstruct records in patterns
- **Pattern Matching for switch (Third Preview)**
- **Foreign Function & Memory API (Preview)**
- **Vector API (Fourth Incubator)**

### Java 20 (March 2023)

- **Scoped Values (Incubator):** Thread-local alternatives
- **Record Patterns (Second Preview)**
- **Pattern Matching for switch (Fourth Preview)**
- **Virtual Threads (Second Preview)**
- **Structured Concurrency (Second Incubator)**
- **Foreign Function & Memory API (Second Preview)**
- **Vector API (Fifth Incubator)**

### Java 21 (LTS - September 2023)

- **Virtual Threads (Standard - Project Loom):** Finalized lightweight threads
- **Record Patterns (Standard):** Finalized feature
- **Pattern Matching for switch (Standard):** Finalized feature
- **Sequenced Collections:** SequencedCollection, SequencedSet, SequencedMap
- **String Templates (Preview):** Embedded expressions in strings
- **Unnamed Patterns and Variables (Preview):** _ for unused variables
- **Unnamed Classes and Instance Main Methods (Preview):** Simplified main
- **Structured Concurrency (Preview)**
- **Scoped Values (Preview)**
- **Foreign Function & Memory API (Third Preview)**
- **Vector API (Sixth Incubator)**
- **Generational ZGC:** Default mode for ZGC
- **Key Encapsulation Mechanism API**

### Java 22 (March 2024)

- **Unnamed Variables & Patterns (Standard):** _ for unused
- **Foreign Function & Memory API (Standard):** Finalized Panama
- **Statements Before super() (Preview):** Code before constructor call
- **String Templates (Second Preview)**
- **Stream Gatherers (Preview):** Custom intermediate operations
- **Structured Concurrency (Second Preview)**
- **Scoped Values (Second Preview)**
- **Class-File API (Preview):** Parse/generate class files
- **Vector API (Seventh Incubator)**
- **Region Pinning for G1:** Reduce latency during JNI

### Java 23 (September 2024)

- **Primitive Types in Patterns (Preview):** Pattern match primitives
- **Module Import Declarations (Preview):** import module java.base
- **Flexible Constructor Bodies (Second Preview)**
- **Stream Gatherers (Second Preview)**
- **Structured Concurrency (Third Preview)**
- **Scoped Values (Third Preview)**
- **Class-File API (Second Preview)**
- **Vector API (Eighth Incubator)**
- **Markdown Documentation Comments**
- **ZGC:** Generational Mode by Default

### Java 24 (March 2025)

- **Stream Gatherers (Standard):** Finalized custom stream operations
- **Class-File API (Standard):** Finalized feature
- **Scoped Values (Standard):** Finalized feature
- **Structured Concurrency (Standard):** Finalized feature
- **Primitive Types in Patterns (Second Preview)**
- **Module Import Declarations (Second Preview)**
- **Flexible Constructor Bodies (Third Preview)**
- **Simple Source Files and Instance Main Methods (Standard)**
- **Ahead-of-Time Class Loading & Linking**
- **Compact Object Headers (Experimental)**
- **Generational Shenandoah (Experimental)**
- **Synchronize Virtual Threads without Pinning**

### Java 25 (LTS - September 2025)

- **Primitive Types in Patterns (Standard):** Finalized pattern matching for primitives
- **Module Import Declarations (Standard):** Finalized module imports
- **Flexible Constructor Bodies (Standard):** Finalized pre-super() statements
- **Vector API (Standard):** Finalized SIMD operations for performance
- **Compact Object Headers (Standard):** Reduced memory footprint for objects
- **Value Classes (Preview):** User-defined primitive-like classes (Project Valhalla)
- **Null-Restricted Types (Preview):** Compile-time null safety
- **Generational Shenandoah (Standard):** Production-ready generational GC
- **Enhanced Pattern Matching:** Improved pattern capabilities
- **Improved Foreign Function & Memory API:** Native interop refinements
- **Project Leyden Improvements:** Faster startup and warmup

---

*Java Version Major Features and Answers*
