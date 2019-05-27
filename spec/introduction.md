# <a name="introduction---test"></a><span data-ttu-id="7eb1a-101">这是一个测试</span><span class="sxs-lookup"><span data-stu-id="7eb1a-101">这是一个测试</span></span>

<span data-ttu-id="7eb1a-102">C# (pronounced "See Sharp") is a simple, modern, object-oriented, and type-safe programming language.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-102">C# (pronounced "See Sharp") is a simple, modern, object-oriented, and type-safe programming language.</span></span> <span data-ttu-id="7eb1a-103">C# has its roots in the C family of languages and will be immediately familiar to C, C++, and Java programmers.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-103">C# has its roots in the C family of languages and will be immediately familiar to C, C++, and Java programmers.</span></span> <span data-ttu-id="7eb1a-104">C# is standardized by ECMA International as the ***ECMA-334*** standard and by ISO/IEC as the ***ISO/IEC 23270*** standard.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-104">C# is standardized by ECMA International as the ***ECMA-334*** standard and by ISO/IEC as the ***ISO/IEC 23270*** standard.</span></span> <span data-ttu-id="7eb1a-105">Microsoft's C# compiler for the .NET Framework is a conforming implementation of both of these standards.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-105">Microsoft's C# compiler for the .NET Framework is a conforming implementation of both of these standards.</span></span>

<span data-ttu-id="7eb1a-106">C# is an object-oriented language, but C# further includes support for ***component-oriented*** programming.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-106">C# is an object-oriented language, but C# further includes support for ***component-oriented*** programming.</span></span> <span data-ttu-id="7eb1a-107">Contemporary software design increasingly relies on software components in the form of self-contained and self-describing packages of functionality.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-107">Contemporary software design increasingly relies on software components in the form of self-contained and self-describing packages of functionality.</span></span> <span data-ttu-id="7eb1a-108">Key to such components is that they present a programming model with properties, methods, and events; they have attributes that provide declarative information about the component; and they incorporate their own documentation.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-108">Key to such components is that they present a programming model with properties, methods, and events; they have attributes that provide declarative information about the component; and they incorporate their own documentation.</span></span> <span data-ttu-id="7eb1a-109">C# provides language constructs to directly support these concepts, making C# a very natural language in which to create and use software components.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-109">C# provides language constructs to directly support these concepts, making C# a very natural language in which to create and use software components.</span></span>

<span data-ttu-id="7eb1a-110">Several C# features aid in the construction of robust and durable applications: ***Garbage collection*** automatically reclaims memory occupied by unused objects; ***exception handling*** provides a structured and extensible approach to error detection and recovery; and the ***type-safe*** design of the language makes it impossible to read from uninitialized variables, to index arrays beyond their bounds, or to perform unchecked type casts.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-110">Several C# features aid in the construction of robust and durable applications: ***Garbage collection*** automatically reclaims memory occupied by unused objects; ***exception handling*** provides a structured and extensible approach to error detection and recovery; and the ***type-safe*** design of the language makes it impossible to read from uninitialized variables, to index arrays beyond their bounds, or to perform unchecked type casts.</span></span>

<span data-ttu-id="7eb1a-111">C# has a ***unified type system***.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-111">C# has a ***unified type system***.</span></span> <span data-ttu-id="7eb1a-112">All C# types, including primitive types such as `int` and `double`, inherit from a single root `object` type.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-112">All C# types, including primitive types such as `int` and `double`, inherit from a single root `object` type.</span></span> <span data-ttu-id="7eb1a-113">Thus, all types share a set of common operations, and values of any type can be stored, transported, and operated upon in a consistent manner.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-113">Thus, all types share a set of common operations, and values of any type can be stored, transported, and operated upon in a consistent manner.</span></span> <span data-ttu-id="7eb1a-114">Furthermore, C# supports both user-defined reference types and value types, allowing dynamic allocation of objects as well as in-line storage of lightweight structures.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-114">Furthermore, C# supports both user-defined reference types and value types, allowing dynamic allocation of objects as well as in-line storage of lightweight structures.</span></span>

<span data-ttu-id="7eb1a-115">To ensure that C# programs and libraries can evolve over time in a compatible manner, much emphasis has been placed on ***versioning*** in C#'s design.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-115">To ensure that C# programs and libraries can evolve over time in a compatible manner, much emphasis has been placed on ***versioning*** in C#'s design.</span></span> <span data-ttu-id="7eb1a-116">Many programming languages pay little attention to this issue, and, as a result, programs written in those languages break more often than necessary when newer versions of dependent libraries are introduced.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-116">Many programming languages pay little attention to this issue, and, as a result, programs written in those languages break more often than necessary when newer versions of dependent libraries are introduced.</span></span> <span data-ttu-id="7eb1a-117">Aspects of C#'s design that were directly influenced by versioning considerations include the separate `virtual` and `override` modifiers, the rules for method overload resolution, and support for explicit interface member declarations.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-117">Aspects of C#'s design that were directly influenced by versioning considerations include the separate `virtual` and `override` modifiers, the rules for method overload resolution, and support for explicit interface member declarations.</span></span>

<span data-ttu-id="7eb1a-118">The rest of this chapter describes the essential features of the C# language.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-118">The rest of this chapter describes the essential features of the C# language.</span></span> <span data-ttu-id="7eb1a-119">Although later chapters describe rules and exceptions in a detail-oriented and sometimes mathematical manner, this chapter strives for clarity and brevity at the expense of completeness.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-119">Although later chapters describe rules and exceptions in a detail-oriented and sometimes mathematical manner, this chapter strives for clarity and brevity at the expense of completeness.</span></span> <span data-ttu-id="7eb1a-120">The intent is to provide the reader with an introduction to the language that will facilitate the writing of early programs and the reading of later chapters.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-120">The intent is to provide the reader with an introduction to the language that will facilitate the writing of early programs and the reading of later chapters.</span></span>

## <a name="hello-world"></a><span data-ttu-id="7eb1a-121">Hello world</span><span class="sxs-lookup"><span data-stu-id="7eb1a-121">Hello world</span></span>

<span data-ttu-id="7eb1a-122">The "Hello, World" program is traditionally used to introduce a programming language.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-122">The "Hello, World" program is traditionally used to introduce a programming language.</span></span> <span data-ttu-id="7eb1a-123">Here it is in C#:</span><span class="sxs-lookup"><span data-stu-id="7eb1a-123">Here it is in C#:</span></span>

```csharp
using System;

class Hello
{
    static void Main() {
        Console.WriteLine("Hello, World");
    }
}
```

<span data-ttu-id="7eb1a-124">C# source files typically have the file extension `.cs`.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-124">C# source files typically have the file extension `.cs`.</span></span> <span data-ttu-id="7eb1a-125">Assuming that the "Hello, World" program is stored in the file `hello.cs`, the program can be compiled with the Microsoft C# compiler using the command line</span><span class="sxs-lookup"><span data-stu-id="7eb1a-125">Assuming that the "Hello, World" program is stored in the file `hello.cs`, the program can be compiled with the Microsoft C# compiler using the command line</span></span>
```
csc hello.cs
```
<span data-ttu-id="7eb1a-126">which produces an executable assembly named `hello.exe`.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-126">which produces an executable assembly named `hello.exe`.</span></span> <span data-ttu-id="7eb1a-127">The output produced by this application when it is run is</span><span class="sxs-lookup"><span data-stu-id="7eb1a-127">The output produced by this application when it is run is</span></span>
```
Hello, World
```

<span data-ttu-id="7eb1a-128">The "Hello, World" program starts with a `using` directive that references the `System` namespace.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-128">The "Hello, World" program starts with a `using` directive that references the `System` namespace.</span></span> <span data-ttu-id="7eb1a-129">Namespaces provide a hierarchical means of organizing C# programs and libraries.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-129">Namespaces provide a hierarchical means of organizing C# programs and libraries.</span></span> <span data-ttu-id="7eb1a-130">Namespaces contain types and other namespaces—for example, the `System` namespace contains a number of types, such as the `Console` class referenced in the program, and a number of other namespaces, such as `IO` and `Collections`.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-130">Namespaces contain types and other namespaces—for example, the `System` namespace contains a number of types, such as the `Console` class referenced in the program, and a number of other namespaces, such as `IO` and `Collections`.</span></span> <span data-ttu-id="7eb1a-131">A `using` directive that references a given namespace enables unqualified use of the types that are members of that namespace.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-131">A `using` directive that references a given namespace enables unqualified use of the types that are members of that namespace.</span></span> <span data-ttu-id="7eb1a-132">Because of the `using` directive, the program can use `Console.WriteLine` as shorthand for `System.Console.WriteLine`.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-132">Because of the `using` directive, the program can use `Console.WriteLine` as shorthand for `System.Console.WriteLine`.</span></span>

<span data-ttu-id="7eb1a-133">The `Hello` class declared by the "Hello, World" program has a single member, the method named `Main`.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-133">The `Hello` class declared by the "Hello, World" program has a single member, the method named `Main`.</span></span> <span data-ttu-id="7eb1a-134">The `Main` method is declared with the `static` modifier.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-134">The `Main` method is declared with the `static` modifier.</span></span> <span data-ttu-id="7eb1a-135">While instance methods can reference a particular enclosing object instance using the keyword `this`, static methods operate without reference to a particular object.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-135">While instance methods can reference a particular enclosing object instance using the keyword `this`, static methods operate without reference to a particular object.</span></span> <span data-ttu-id="7eb1a-136">By convention, a static method named `Main` serves as the entry point of a program.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-136">By convention, a static method named `Main` serves as the entry point of a program.</span></span>

<span data-ttu-id="7eb1a-137">The output of the program is produced by the `WriteLine` method of the `Console` class in the `System` namespace.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-137">The output of the program is produced by the `WriteLine` method of the `Console` class in the `System` namespace.</span></span> <span data-ttu-id="7eb1a-138">This class is provided by the .NET Framework class libraries, which, by default, are automatically referenced by the Microsoft C# compiler.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-138">This class is provided by the .NET Framework class libraries, which, by default, are automatically referenced by the Microsoft C# compiler.</span></span> <span data-ttu-id="7eb1a-139">Note that C# itself does not have a separate runtime library.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-139">Note that C# itself does not have a separate runtime library.</span></span> <span data-ttu-id="7eb1a-140">Instead, the .NET Framework is the runtime library of C#.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-140">Instead, the .NET Framework is the runtime library of C#.</span></span>

## <a name="program-structure"></a><span data-ttu-id="7eb1a-141">Program structure</span><span class="sxs-lookup"><span data-stu-id="7eb1a-141">Program structure</span></span>

<span data-ttu-id="7eb1a-142">The key organizational concepts in C# are ***programs***, ***namespaces***, ***types***, ***members***, and ***assemblies***.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-142">The key organizational concepts in C# are ***programs***, ***namespaces***, ***types***, ***members***, and ***assemblies***.</span></span> <span data-ttu-id="7eb1a-143">C# programs consist of one or more source files.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-143">C# programs consist of one or more source files.</span></span> <span data-ttu-id="7eb1a-144">Programs declare types, which contain members and can be organized into namespaces.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-144">Programs declare types, which contain members and can be organized into namespaces.</span></span> <span data-ttu-id="7eb1a-145">Classes and interfaces are examples of types.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-145">Classes and interfaces are examples of types.</span></span> <span data-ttu-id="7eb1a-146">Fields, methods, properties, and events are examples of members.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-146">Fields, methods, properties, and events are examples of members.</span></span> <span data-ttu-id="7eb1a-147">When C# programs are compiled, they are physically packaged into assemblies.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-147">When C# programs are compiled, they are physically packaged into assemblies.</span></span> <span data-ttu-id="7eb1a-148">Assemblies typically have the file extension `.exe` or `.dll`, depending on whether they implement ***applications*** or ***libraries***.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-148">Assemblies typically have the file extension `.exe` or `.dll`, depending on whether they implement ***applications*** or ***libraries***.</span></span>

<span data-ttu-id="7eb1a-149">The example</span><span class="sxs-lookup"><span data-stu-id="7eb1a-149">The example</span></span>

```csharp
using System;

namespace Acme.Collections
{
    public class Stack
    {
        Entry top;

        public void Push(object data) {
            top = new Entry(top, data);
        }

        public object Pop() {
            if (top == null) throw new InvalidOperationException();
            object result = top.data;
            top = top.next;
            return result;
        }

        class Entry
        {
            public Entry next;
            public object data;
    
            public Entry(Entry next, object data) {
                this.next = next;
                this.data = data;
            }
        }
    }
}
```
<span data-ttu-id="7eb1a-150">declares a class named `Stack` in a namespace called `Acme.Collections`.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-150">declares a class named `Stack` in a namespace called `Acme.Collections`.</span></span> <span data-ttu-id="7eb1a-151">The fully qualified name of this class is `Acme.Collections.Stack`.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-151">The fully qualified name of this class is `Acme.Collections.Stack`.</span></span> <span data-ttu-id="7eb1a-152">The class contains several members: a field named `top`, two methods named `Push` and `Pop`, and a nested class named `Entry`.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-152">The class contains several members: a field named `top`, two methods named `Push` and `Pop`, and a nested class named `Entry`.</span></span> <span data-ttu-id="7eb1a-153">The `Entry` class further contains three members: a field named `next`, a field named `data`, and a constructor.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-153">The `Entry` class further contains three members: a field named `next`, a field named `data`, and a constructor.</span></span> <span data-ttu-id="7eb1a-154">Assuming that the source code of the example is stored in the file `acme.cs`, the command line</span><span class="sxs-lookup"><span data-stu-id="7eb1a-154">Assuming that the source code of the example is stored in the file `acme.cs`, the command line</span></span>

```
csc /t:library acme.cs
```
<span data-ttu-id="7eb1a-155">compiles the example as a library (code without a `Main` entry point) and produces an assembly named `acme.dll`.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-155">compiles the example as a library (code without a `Main` entry point) and produces an assembly named `acme.dll`.</span></span>

<span data-ttu-id="7eb1a-156">Assemblies contain executable code in the form of ***Intermediate Language*** (IL) instructions, and symbolic information in the form of ***metadata***.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-156">Assemblies contain executable code in the form of ***Intermediate Language*** (IL) instructions, and symbolic information in the form of ***metadata***.</span></span> <span data-ttu-id="7eb1a-157">Before it is executed, the IL code in an assembly is automatically converted to processor-specific code by the Just-In-Time (JIT) compiler of .NET Common Language Runtime.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-157">Before it is executed, the IL code in an assembly is automatically converted to processor-specific code by the Just-In-Time (JIT) compiler of .NET Common Language Runtime.</span></span>

<span data-ttu-id="7eb1a-158">Because an assembly is a self-describing unit of functionality containing both code and metadata, there is no need for `#include` directives and header files in C#.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-158">Because an assembly is a self-describing unit of functionality containing both code and metadata, there is no need for `#include` directives and header files in C#.</span></span> <span data-ttu-id="7eb1a-159">The public types and members contained in a particular assembly are made available in a C# program simply by referencing that assembly when compiling the program.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-159">The public types and members contained in a particular assembly are made available in a C# program simply by referencing that assembly when compiling the program.</span></span> <span data-ttu-id="7eb1a-160">For example, this program uses the `Acme.Collections.Stack` class from the `acme.dll` assembly:</span><span class="sxs-lookup"><span data-stu-id="7eb1a-160">For example, this program uses the `Acme.Collections.Stack` class from the `acme.dll` assembly:</span></span>

```csharp
using System;
using Acme.Collections;

class Test
{
    static void Main() {
        Stack s = new Stack();
        s.Push(1);
        s.Push(10);
        s.Push(100);
        Console.WriteLine(s.Pop());
        Console.WriteLine(s.Pop());
        Console.WriteLine(s.Pop());
    }
}
```
<span data-ttu-id="7eb1a-161">If the program is stored in the file `test.cs`, when `test.cs` is compiled, the `acme.dll` assembly can be referenced using the compiler's `/r` option:</span><span class="sxs-lookup"><span data-stu-id="7eb1a-161">If the program is stored in the file `test.cs`, when `test.cs` is compiled, the `acme.dll` assembly can be referenced using the compiler's `/r` option:</span></span>

```
csc /r:acme.dll test.cs
```
<span data-ttu-id="7eb1a-162">This creates an executable assembly named `test.exe`, which, when run, produces the output:</span><span class="sxs-lookup"><span data-stu-id="7eb1a-162">This creates an executable assembly named `test.exe`, which, when run, produces the output:</span></span>

```
100
10
1
```
<span data-ttu-id="7eb1a-163">C# permits the source text of a program to be stored in several source files.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-163">C# permits the source text of a program to be stored in several source files.</span></span> <span data-ttu-id="7eb1a-164">When a multi-file C# program is compiled, all of the source files are processed together, and the source files can freely reference each other—conceptually, it is as if all the source files were concatenated into one large file before being processed.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-164">When a multi-file C# program is compiled, all of the source files are processed together, and the source files can freely reference each other—conceptually, it is as if all the source files were concatenated into one large file before being processed.</span></span> <span data-ttu-id="7eb1a-165">Forward declarations are never needed in C# because, with very few exceptions, declaration order is insignificant.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-165">Forward declarations are never needed in C# because, with very few exceptions, declaration order is insignificant.</span></span> <span data-ttu-id="7eb1a-166">C# does not limit a source file to declaring only one public type nor does it require the name of the source file to match a type declared in the source file.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-166">C# does not limit a source file to declaring only one public type nor does it require the name of the source file to match a type declared in the source file.</span></span>

## <a name="types-and-variables"></a><span data-ttu-id="7eb1a-167">Types and variables</span><span class="sxs-lookup"><span data-stu-id="7eb1a-167">Types and variables</span></span>

<span data-ttu-id="7eb1a-168">There are two kinds of types in C#: ***value types*** and ***reference types***.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-168">There are two kinds of types in C#: ***value types*** and ***reference types***.</span></span> <span data-ttu-id="7eb1a-169">Variables of value types directly contain their data whereas variables of reference types store references to their data, the latter being known as objects.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-169">Variables of value types directly contain their data whereas variables of reference types store references to their data, the latter being known as objects.</span></span> <span data-ttu-id="7eb1a-170">With reference types, it is possible for two variables to reference the same object and thus possible for operations on one variable to affect the object referenced by the other variable.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-170">With reference types, it is possible for two variables to reference the same object and thus possible for operations on one variable to affect the object referenced by the other variable.</span></span> <span data-ttu-id="7eb1a-171">With value types, the variables each have their own copy of the data, and it is not possible for operations on one to affect the other (except in the case of `ref` and `out` parameter variables).</span><span class="sxs-lookup"><span data-stu-id="7eb1a-171">With value types, the variables each have their own copy of the data, and it is not possible for operations on one to affect the other (except in the case of `ref` and `out` parameter variables).</span></span>

<span data-ttu-id="7eb1a-172">C#'s value types are further divided into ***simple types***, ***enum types***, ***struct types***, and ***nullable types***, and C#'s reference types are further divided into ***class types***, ***interface types***, ***array types***, and ***delegate types***.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-172">C#'s value types are further divided into ***simple types***, ***enum types***, ***struct types***, and ***nullable types***, and C#'s reference types are further divided into ***class types***, ***interface types***, ***array types***, and ***delegate types***.</span></span>

<span data-ttu-id="7eb1a-173">The following table provides an overview of C#'s type system.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-173">The following table provides an overview of C#'s type system.</span></span>

| <span data-ttu-id="7eb1a-174">__Category__</span><span class="sxs-lookup"><span data-stu-id="7eb1a-174">__Category__</span></span>    |                 | <span data-ttu-id="7eb1a-175">__Description__</span><span class="sxs-lookup"><span data-stu-id="7eb1a-175">__Description__</span></span> |
|-----------------|-----------------|-----------------|
| <span data-ttu-id="7eb1a-176">Value types</span><span class="sxs-lookup"><span data-stu-id="7eb1a-176">Value types</span></span>     | <span data-ttu-id="7eb1a-177">Simple types</span><span class="sxs-lookup"><span data-stu-id="7eb1a-177">Simple types</span></span>    | <span data-ttu-id="7eb1a-178">Signed integral: `sbyte`, `short`, `int`, `long`</span><span class="sxs-lookup"><span data-stu-id="7eb1a-178">Signed integral: `sbyte`, `short`, `int`, `long`</span></span> |
|                 |                 | <span data-ttu-id="7eb1a-179">Unsigned integral: `byte`, `ushort`, `uint`, `ulong`</span><span class="sxs-lookup"><span data-stu-id="7eb1a-179">Unsigned integral: `byte`, `ushort`, `uint`, `ulong`</span></span> |
|                 |                 | <span data-ttu-id="7eb1a-180">Unicode characters: `char`</span><span class="sxs-lookup"><span data-stu-id="7eb1a-180">Unicode characters: `char`</span></span> |
|                 |                 | <span data-ttu-id="7eb1a-181">IEEE floating point: `float`, `double`</span><span class="sxs-lookup"><span data-stu-id="7eb1a-181">IEEE floating point: `float`, `double`</span></span> |
|                 |                 | <span data-ttu-id="7eb1a-182">High-precision decimal: `decimal`</span><span class="sxs-lookup"><span data-stu-id="7eb1a-182">High-precision decimal: `decimal`</span></span> |
|                 |                 | <span data-ttu-id="7eb1a-183">Boolean: `bool`</span><span class="sxs-lookup"><span data-stu-id="7eb1a-183">Boolean: `bool`</span></span> |
|                 | <span data-ttu-id="7eb1a-184">Enum types</span><span class="sxs-lookup"><span data-stu-id="7eb1a-184">Enum types</span></span>      | <span data-ttu-id="7eb1a-185">User-defined types of the form `enum E {...}`</span><span class="sxs-lookup"><span data-stu-id="7eb1a-185">User-defined types of the form `enum E {...}`</span></span> |
|                 | <span data-ttu-id="7eb1a-186">Struct types</span><span class="sxs-lookup"><span data-stu-id="7eb1a-186">Struct types</span></span>    | <span data-ttu-id="7eb1a-187">User-defined types of the form `struct S {...}`</span><span class="sxs-lookup"><span data-stu-id="7eb1a-187">User-defined types of the form `struct S {...}`</span></span> |
|                 | <span data-ttu-id="7eb1a-188">Nullable types</span><span class="sxs-lookup"><span data-stu-id="7eb1a-188">Nullable types</span></span>  | <span data-ttu-id="7eb1a-189">Extensions of all other value types with a `null` value</span><span class="sxs-lookup"><span data-stu-id="7eb1a-189">Extensions of all other value types with a `null` value</span></span> |
| <span data-ttu-id="7eb1a-190">Reference types</span><span class="sxs-lookup"><span data-stu-id="7eb1a-190">Reference types</span></span> | <span data-ttu-id="7eb1a-191">Class types</span><span class="sxs-lookup"><span data-stu-id="7eb1a-191">Class types</span></span>     | <span data-ttu-id="7eb1a-192">Ultimate base class of all other types: `object`</span><span class="sxs-lookup"><span data-stu-id="7eb1a-192">Ultimate base class of all other types: `object`</span></span> |
|                 |                 | <span data-ttu-id="7eb1a-193">Unicode strings: `string`</span><span class="sxs-lookup"><span data-stu-id="7eb1a-193">Unicode strings: `string`</span></span> |
|                 |                 | <span data-ttu-id="7eb1a-194">User-defined types of the form `class C {...}`</span><span class="sxs-lookup"><span data-stu-id="7eb1a-194">User-defined types of the form `class C {...}`</span></span> |
|                 | <span data-ttu-id="7eb1a-195">Interface types</span><span class="sxs-lookup"><span data-stu-id="7eb1a-195">Interface types</span></span> | <span data-ttu-id="7eb1a-196">User-defined types of the form `interface I {...}`</span><span class="sxs-lookup"><span data-stu-id="7eb1a-196">User-defined types of the form `interface I {...}`</span></span> |
|                 | <span data-ttu-id="7eb1a-197">Array types</span><span class="sxs-lookup"><span data-stu-id="7eb1a-197">Array types</span></span>     | <span data-ttu-id="7eb1a-198">Single- and multi-dimensional, for example, `int[]` and `int[,]`</span><span class="sxs-lookup"><span data-stu-id="7eb1a-198">Single- and multi-dimensional, for example, `int[]` and `int[,]`</span></span> |
|                 | <span data-ttu-id="7eb1a-199">Delegate types</span><span class="sxs-lookup"><span data-stu-id="7eb1a-199">Delegate types</span></span>  | <span data-ttu-id="7eb1a-200">User-defined types of the form e.g. `delegate int  D(...)`</span><span class="sxs-lookup"><span data-stu-id="7eb1a-200">User-defined types of the form e.g. `delegate int  D(...)`</span></span> |

<span data-ttu-id="7eb1a-201">The eight integral types provide support for 8-bit, 16-bit, 32-bit, and 64-bit values in signed or unsigned form.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-201">The eight integral types provide support for 8-bit, 16-bit, 32-bit, and 64-bit values in signed or unsigned form.</span></span>

<span data-ttu-id="7eb1a-202">The two floating point types, `float` and `double`, are represented using the 32-bit single-precision and 64-bit double-precision IEEE 754 formats.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-202">The two floating point types, `float` and `double`, are represented using the 32-bit single-precision and 64-bit double-precision IEEE 754 formats.</span></span>

<span data-ttu-id="7eb1a-203">The `decimal` type is a 128-bit data type suitable for financial and monetary calculations.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-203">The `decimal` type is a 128-bit data type suitable for financial and monetary calculations.</span></span>

<span data-ttu-id="7eb1a-204">C#'s `bool` type is used to represent boolean values—values that are either `true` or `false`.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-204">C#'s `bool` type is used to represent boolean values—values that are either `true` or `false`.</span></span>

<span data-ttu-id="7eb1a-205">Character and string processing in C# uses Unicode encoding.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-205">Character and string processing in C# uses Unicode encoding.</span></span> <span data-ttu-id="7eb1a-206">The `char` type represents a UTF-16 code unit, and the `string` type represents a sequence of UTF-16 code units.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-206">The `char` type represents a UTF-16 code unit, and the `string` type represents a sequence of UTF-16 code units.</span></span>

<span data-ttu-id="7eb1a-207">The following table summarizes C#'s numeric types.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-207">The following table summarizes C#'s numeric types.</span></span>


| <span data-ttu-id="7eb1a-208">__Category__</span><span class="sxs-lookup"><span data-stu-id="7eb1a-208">__Category__</span></span>      | <span data-ttu-id="7eb1a-209">__Bits__</span><span class="sxs-lookup"><span data-stu-id="7eb1a-209">__Bits__</span></span> | <span data-ttu-id="7eb1a-210">__Type__</span><span class="sxs-lookup"><span data-stu-id="7eb1a-210">__Type__</span></span>  | <span data-ttu-id="7eb1a-211">__Range/Precision__</span><span class="sxs-lookup"><span data-stu-id="7eb1a-211">__Range/Precision__</span></span> |
|-------------------|----------|-----------|---------------------|
| <span data-ttu-id="7eb1a-212">Signed integral</span><span class="sxs-lookup"><span data-stu-id="7eb1a-212">Signed integral</span></span>   | <span data-ttu-id="7eb1a-213">8</span><span class="sxs-lookup"><span data-stu-id="7eb1a-213">8</span></span>        | `sbyte`   | <span data-ttu-id="7eb1a-214">-128...127</span><span class="sxs-lookup"><span data-stu-id="7eb1a-214">-128...127</span></span> |
|                   | <span data-ttu-id="7eb1a-215">16</span><span class="sxs-lookup"><span data-stu-id="7eb1a-215">16</span></span>       | `short`   | <span data-ttu-id="7eb1a-216">-32,768...32,767</span><span class="sxs-lookup"><span data-stu-id="7eb1a-216">-32,768...32,767</span></span> |
|                   | <span data-ttu-id="7eb1a-217">32</span><span class="sxs-lookup"><span data-stu-id="7eb1a-217">32</span></span>       | `int`     | <span data-ttu-id="7eb1a-218">-2,147,483,648...2,147,483,647</span><span class="sxs-lookup"><span data-stu-id="7eb1a-218">-2,147,483,648...2,147,483,647</span></span> |
|                   | <span data-ttu-id="7eb1a-219">64</span><span class="sxs-lookup"><span data-stu-id="7eb1a-219">64</span></span>       | `long`    | <span data-ttu-id="7eb1a-220">-9,223,372,036,854,775,808...9,223,372,036,854,775,807</span><span class="sxs-lookup"><span data-stu-id="7eb1a-220">-9,223,372,036,854,775,808...9,223,372,036,854,775,807</span></span> |
| <span data-ttu-id="7eb1a-221">Unsigned integral</span><span class="sxs-lookup"><span data-stu-id="7eb1a-221">Unsigned integral</span></span> | <span data-ttu-id="7eb1a-222">8</span><span class="sxs-lookup"><span data-stu-id="7eb1a-222">8</span></span>        | `byte`    | <span data-ttu-id="7eb1a-223">0...255</span><span class="sxs-lookup"><span data-stu-id="7eb1a-223">0...255</span></span> |
|                   | <span data-ttu-id="7eb1a-224">16</span><span class="sxs-lookup"><span data-stu-id="7eb1a-224">16</span></span>       | `ushort`  | <span data-ttu-id="7eb1a-225">0...65,535</span><span class="sxs-lookup"><span data-stu-id="7eb1a-225">0...65,535</span></span> |
|                   | <span data-ttu-id="7eb1a-226">32</span><span class="sxs-lookup"><span data-stu-id="7eb1a-226">32</span></span>       | `uint`    | <span data-ttu-id="7eb1a-227">0...4,294,967,295</span><span class="sxs-lookup"><span data-stu-id="7eb1a-227">0...4,294,967,295</span></span> |
|                   | <span data-ttu-id="7eb1a-228">64</span><span class="sxs-lookup"><span data-stu-id="7eb1a-228">64</span></span>       | `ulong`   | <span data-ttu-id="7eb1a-229">0...18,446,744,073,709,551,615</span><span class="sxs-lookup"><span data-stu-id="7eb1a-229">0...18,446,744,073,709,551,615</span></span> |
| <span data-ttu-id="7eb1a-230">Floating point</span><span class="sxs-lookup"><span data-stu-id="7eb1a-230">Floating point</span></span>    | <span data-ttu-id="7eb1a-231">32</span><span class="sxs-lookup"><span data-stu-id="7eb1a-231">32</span></span>       | `float`   | <span data-ttu-id="7eb1a-232">1.5 × 10^−45 to 3.4 × 10^38, 7-digit precision</span><span class="sxs-lookup"><span data-stu-id="7eb1a-232">1.5 × 10^−45 to 3.4 × 10^38, 7-digit precision</span></span> |
|                   | <span data-ttu-id="7eb1a-233">64</span><span class="sxs-lookup"><span data-stu-id="7eb1a-233">64</span></span>       | `double`  | <span data-ttu-id="7eb1a-234">5.0 × 10^−324 to 1.7 × 10^308, 15-digit precision</span><span class="sxs-lookup"><span data-stu-id="7eb1a-234">5.0 × 10^−324 to 1.7 × 10^308, 15-digit precision</span></span> |
| <span data-ttu-id="7eb1a-235">Decimal</span><span class="sxs-lookup"><span data-stu-id="7eb1a-235">Decimal</span></span>           | <span data-ttu-id="7eb1a-236">128</span><span class="sxs-lookup"><span data-stu-id="7eb1a-236">128</span></span>      | `decimal` | <span data-ttu-id="7eb1a-237">1.0 × 10^−28 to 7.9 × 10^28, 28-digit precision</span><span class="sxs-lookup"><span data-stu-id="7eb1a-237">1.0 × 10^−28 to 7.9 × 10^28, 28-digit precision</span></span> |

<span data-ttu-id="7eb1a-238">C# programs use ***type declarations*** to create new types.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-238">C# programs use ***type declarations*** to create new types.</span></span> <span data-ttu-id="7eb1a-239">A type declaration specifies the name and the members of the new type.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-239">A type declaration specifies the name and the members of the new type.</span></span> <span data-ttu-id="7eb1a-240">Five of C#'s categories of types are user-definable: class types, struct types, interface types, enum types, and delegate types.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-240">Five of C#'s categories of types are user-definable: class types, struct types, interface types, enum types, and delegate types.</span></span>

<span data-ttu-id="7eb1a-241">A class type defines a data structure that contains data members (fields) and function members (methods, properties, and others).</span><span class="sxs-lookup"><span data-stu-id="7eb1a-241">A class type defines a data structure that contains data members (fields) and function members (methods, properties, and others).</span></span> <span data-ttu-id="7eb1a-242">Class types support single inheritance and polymorphism, mechanisms whereby derived classes can extend and specialize base classes.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-242">Class types support single inheritance and polymorphism, mechanisms whereby derived classes can extend and specialize base classes.</span></span>

<span data-ttu-id="7eb1a-243">A struct type is similar to a class type in that it represents a structure with data members and function members.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-243">A struct type is similar to a class type in that it represents a structure with data members and function members.</span></span> <span data-ttu-id="7eb1a-244">However, unlike classes, structs are value types and do not require heap allocation.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-244">However, unlike classes, structs are value types and do not require heap allocation.</span></span> <span data-ttu-id="7eb1a-245">Struct types do not support user-specified inheritance, and all struct types implicitly inherit from type `object`.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-245">Struct types do not support user-specified inheritance, and all struct types implicitly inherit from type `object`.</span></span>

<span data-ttu-id="7eb1a-246">An interface type defines a contract as a named set of public function members.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-246">An interface type defines a contract as a named set of public function members.</span></span> <span data-ttu-id="7eb1a-247">A class or struct that implements an interface must provide implementations of the interface's function members.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-247">A class or struct that implements an interface must provide implementations of the interface's function members.</span></span> <span data-ttu-id="7eb1a-248">An interface may inherit from multiple base interfaces, and a class or struct may implement multiple interfaces.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-248">An interface may inherit from multiple base interfaces, and a class or struct may implement multiple interfaces.</span></span>

<span data-ttu-id="7eb1a-249">A delegate type represents references to methods with a particular parameter list and return type.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-249">A delegate type represents references to methods with a particular parameter list and return type.</span></span> <span data-ttu-id="7eb1a-250">Delegates make it possible to treat methods as entities that can be assigned to variables and passed as parameters.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-250">Delegates make it possible to treat methods as entities that can be assigned to variables and passed as parameters.</span></span> <span data-ttu-id="7eb1a-251">Delegates are similar to the concept of function pointers found in some other languages, but unlike function pointers, delegates are object-oriented and type-safe.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-251">Delegates are similar to the concept of function pointers found in some other languages, but unlike function pointers, delegates are object-oriented and type-safe.</span></span>

<span data-ttu-id="7eb1a-252">Class, struct, interface and delegate types all support generics, whereby they can be parameterized with other types.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-252">Class, struct, interface and delegate types all support generics, whereby they can be parameterized with other types.</span></span>

<span data-ttu-id="7eb1a-253">An enum type is a distinct type with named constants.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-253">An enum type is a distinct type with named constants.</span></span> <span data-ttu-id="7eb1a-254">Every enum type has an underlying type, which must be one of the eight integral types.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-254">Every enum type has an underlying type, which must be one of the eight integral types.</span></span> <span data-ttu-id="7eb1a-255">The set of values of an enum type is the same as the set of values of the underlying type.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-255">The set of values of an enum type is the same as the set of values of the underlying type.</span></span>

<span data-ttu-id="7eb1a-256">C# supports single- and multi-dimensional arrays of any type.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-256">C# supports single- and multi-dimensional arrays of any type.</span></span> <span data-ttu-id="7eb1a-257">Unlike the types listed above, array types do not have to be declared before they can be used.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-257">Unlike the types listed above, array types do not have to be declared before they can be used.</span></span> <span data-ttu-id="7eb1a-258">Instead, array types are constructed by following a type name with square brackets.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-258">Instead, array types are constructed by following a type name with square brackets.</span></span> <span data-ttu-id="7eb1a-259">For example, `int[]` is a single-dimensional array of `int`, `int[,]` is a two-dimensional array of `int`, and `int[][]` is a single-dimensional array of single-dimensional arrays of `int`.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-259">For example, `int[]` is a single-dimensional array of `int`, `int[,]` is a two-dimensional array of `int`, and `int[][]` is a single-dimensional array of single-dimensional arrays of `int`.</span></span>

<span data-ttu-id="7eb1a-260">Nullable types also do not have to be declared before they can be used.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-260">Nullable types also do not have to be declared before they can be used.</span></span> <span data-ttu-id="7eb1a-261">For each non-nullable value type `T` there is a corresponding nullable type `T?`, which can hold an additional value `null`.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-261">For each non-nullable value type `T` there is a corresponding nullable type `T?`, which can hold an additional value `null`.</span></span> <span data-ttu-id="7eb1a-262">For instance, `int?` is a type that can hold any 32 bit integer or the value `null`.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-262">For instance, `int?` is a type that can hold any 32 bit integer or the value `null`.</span></span>

<span data-ttu-id="7eb1a-263">C#'s type system is unified such that a value of any type can be treated as an object.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-263">C#'s type system is unified such that a value of any type can be treated as an object.</span></span> <span data-ttu-id="7eb1a-264">Every type in C# directly or indirectly derives from the `object` class type, and `object` is the ultimate base class of all types.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-264">Every type in C# directly or indirectly derives from the `object` class type, and `object` is the ultimate base class of all types.</span></span> <span data-ttu-id="7eb1a-265">Values of reference types are treated as objects simply by viewing the values as type `object`.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-265">Values of reference types are treated as objects simply by viewing the values as type `object`.</span></span> <span data-ttu-id="7eb1a-266">Values of value types are treated as objects by performing ***boxing*** and ***unboxing*** operations.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-266">Values of value types are treated as objects by performing ***boxing*** and ***unboxing*** operations.</span></span> <span data-ttu-id="7eb1a-267">In the following example, an `int` value is converted to `object` and back again to `int`.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-267">In the following example, an `int` value is converted to `object` and back again to `int`.</span></span>

```csharp
using System;

class Test
{
    static void Main() {
        int i = 123;
        object o = i;          // Boxing
        int j = (int)o;        // Unboxing
    }
}
```
<span data-ttu-id="7eb1a-268">When a value of a value type is converted to type `object`, an object instance, also called a "box," is allocated to hold the value, and the value is copied into that box.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-268">When a value of a value type is converted to type `object`, an object instance, also called a "box," is allocated to hold the value, and the value is copied into that box.</span></span> <span data-ttu-id="7eb1a-269">Conversely, when an `object` reference is cast to a value type, a check is made that the referenced object is a box of the correct value type, and, if the check succeeds, the value in the box is copied out.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-269">Conversely, when an `object` reference is cast to a value type, a check is made that the referenced object is a box of the correct value type, and, if the check succeeds, the value in the box is copied out.</span></span>

<span data-ttu-id="7eb1a-270">C#'s unified type system effectively means that value types can become objects "on demand."</span><span class="sxs-lookup"><span data-stu-id="7eb1a-270">C#'s unified type system effectively means that value types can become objects "on demand."</span></span> <span data-ttu-id="7eb1a-271">Because of the unification, general-purpose libraries that use type `object` can be used with both reference types and value types.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-271">Because of the unification, general-purpose libraries that use type `object` can be used with both reference types and value types.</span></span>

<span data-ttu-id="7eb1a-272">There are several kinds of ***variables*** in C#, including fields, array elements, local variables, and parameters.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-272">There are several kinds of ***variables*** in C#, including fields, array elements, local variables, and parameters.</span></span> <span data-ttu-id="7eb1a-273">Variables represent storage locations, and every variable has a type that determines what values can be stored in the variable, as shown by the following table.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-273">Variables represent storage locations, and every variable has a type that determines what values can be stored in the variable, as shown by the following table.</span></span>


| <span data-ttu-id="7eb1a-274">__Type of Variable__</span><span class="sxs-lookup"><span data-stu-id="7eb1a-274">__Type of Variable__</span></span>    | <span data-ttu-id="7eb1a-275">__Possible Contents__</span><span class="sxs-lookup"><span data-stu-id="7eb1a-275">__Possible Contents__</span></span> |
|-------------------------|-----------------------|
| <span data-ttu-id="7eb1a-276">Non-nullable value type</span><span class="sxs-lookup"><span data-stu-id="7eb1a-276">Non-nullable value type</span></span> | <span data-ttu-id="7eb1a-277">A value of that exact type</span><span class="sxs-lookup"><span data-stu-id="7eb1a-277">A value of that exact type</span></span> |
| <span data-ttu-id="7eb1a-278">Nullable value type</span><span class="sxs-lookup"><span data-stu-id="7eb1a-278">Nullable value type</span></span>     | <span data-ttu-id="7eb1a-279">A null value or a value of that exact type</span><span class="sxs-lookup"><span data-stu-id="7eb1a-279">A null value or a value of that exact type</span></span> |
| `object`                | <span data-ttu-id="7eb1a-280">A null reference, a reference to an object of any reference type, or a reference to a boxed value of any value type</span><span class="sxs-lookup"><span data-stu-id="7eb1a-280">A null reference, a reference to an object of any reference type, or a reference to a boxed value of any value type</span></span> |
| <span data-ttu-id="7eb1a-281">Class type</span><span class="sxs-lookup"><span data-stu-id="7eb1a-281">Class type</span></span>              | <span data-ttu-id="7eb1a-282">A null reference, a reference to an instance of that class type, or a reference to an instance of a class derived from that class type</span><span class="sxs-lookup"><span data-stu-id="7eb1a-282">A null reference, a reference to an instance of that class type, or a reference to an instance of a class derived from that class type</span></span> |
| <span data-ttu-id="7eb1a-283">Interface type</span><span class="sxs-lookup"><span data-stu-id="7eb1a-283">Interface type</span></span>          | <span data-ttu-id="7eb1a-284">A null reference, a reference to an instance of a class type that implements that interface type, or a reference to a boxed value of a value type that implements that interface type</span><span class="sxs-lookup"><span data-stu-id="7eb1a-284">A null reference, a reference to an instance of a class type that implements that interface type, or a reference to a boxed value of a value type that implements that interface type</span></span> |
| <span data-ttu-id="7eb1a-285">Array type</span><span class="sxs-lookup"><span data-stu-id="7eb1a-285">Array type</span></span>              | <span data-ttu-id="7eb1a-286">A null reference, a reference to an instance of that array type, or a reference to an instance of a compatible array type</span><span class="sxs-lookup"><span data-stu-id="7eb1a-286">A null reference, a reference to an instance of that array type, or a reference to an instance of a compatible array type</span></span> |
| <span data-ttu-id="7eb1a-287">Delegate type</span><span class="sxs-lookup"><span data-stu-id="7eb1a-287">Delegate type</span></span>           | <span data-ttu-id="7eb1a-288">A null reference or a reference to an instance of that delegate type</span><span class="sxs-lookup"><span data-stu-id="7eb1a-288">A null reference or a reference to an instance of that delegate type</span></span> |

## <a name="expressions"></a><span data-ttu-id="7eb1a-289">Expressions</span><span class="sxs-lookup"><span data-stu-id="7eb1a-289">Expressions</span></span>

<span data-ttu-id="7eb1a-290">***Expressions*** are constructed from ***operands*** and ***operators***.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-290">***Expressions*** are constructed from ***operands*** and ***operators***.</span></span> <span data-ttu-id="7eb1a-291">The operators of an expression indicate which operations to apply to the operands.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-291">The operators of an expression indicate which operations to apply to the operands.</span></span> <span data-ttu-id="7eb1a-292">Examples of operators include `+`, `-`, `*`, `/`, and `new`.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-292">Examples of operators include `+`, `-`, `*`, `/`, and `new`.</span></span> <span data-ttu-id="7eb1a-293">Examples of operands include literals, fields, local variables, and expressions.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-293">Examples of operands include literals, fields, local variables, and expressions.</span></span>

<span data-ttu-id="7eb1a-294">When an expression contains multiple operators, the ***precedence*** of the operators controls the order in which the individual operators are evaluated.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-294">When an expression contains multiple operators, the ***precedence*** of the operators controls the order in which the individual operators are evaluated.</span></span> <span data-ttu-id="7eb1a-295">For example, the expression `x + y * z` is evaluated as `x + (y * z)` because the `*` operator has higher precedence than the `+` operator.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-295">For example, the expression `x + y * z` is evaluated as `x + (y * z)` because the `*` operator has higher precedence than the `+` operator.</span></span>

<span data-ttu-id="7eb1a-296">Most operators can be ***overloaded***.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-296">Most operators can be ***overloaded***.</span></span> <span data-ttu-id="7eb1a-297">Operator overloading permits user-defined operator implementations to be specified for operations where one or both of the operands are of a user-defined class or struct type.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-297">Operator overloading permits user-defined operator implementations to be specified for operations where one or both of the operands are of a user-defined class or struct type.</span></span>

<span data-ttu-id="7eb1a-298">The following table summarizes C#'s operators, listing the operator categories in order of precedence from highest to lowest.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-298">The following table summarizes C#'s operators, listing the operator categories in order of precedence from highest to lowest.</span></span> <span data-ttu-id="7eb1a-299">Operators in the same category have equal precedence.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-299">Operators in the same category have equal precedence.</span></span>


| <span data-ttu-id="7eb1a-300">__Category__</span><span class="sxs-lookup"><span data-stu-id="7eb1a-300">__Category__</span></span>                     | <span data-ttu-id="7eb1a-301">__Expression__</span><span class="sxs-lookup"><span data-stu-id="7eb1a-301">__Expression__</span></span>    | <span data-ttu-id="7eb1a-302">__Description__</span><span class="sxs-lookup"><span data-stu-id="7eb1a-302">__Description__</span></span> |
|----------------------------------|-------------------|-----------------|
| <span data-ttu-id="7eb1a-303">Primary</span><span class="sxs-lookup"><span data-stu-id="7eb1a-303">Primary</span></span>                          | `x.m`             | <span data-ttu-id="7eb1a-304">Member access</span><span class="sxs-lookup"><span data-stu-id="7eb1a-304">Member access</span></span> |
|                                  | `x(...)`          | <span data-ttu-id="7eb1a-305">Method and delegate invocation</span><span class="sxs-lookup"><span data-stu-id="7eb1a-305">Method and delegate invocation</span></span> |
|                                  | `x[...]`          | <span data-ttu-id="7eb1a-306">Array and indexer access</span><span class="sxs-lookup"><span data-stu-id="7eb1a-306">Array and indexer access</span></span> |
|                                  | `x++`             | <span data-ttu-id="7eb1a-307">Post-increment</span><span class="sxs-lookup"><span data-stu-id="7eb1a-307">Post-increment</span></span> |
|                                  | `x--`             | <span data-ttu-id="7eb1a-308">Post-decrement</span><span class="sxs-lookup"><span data-stu-id="7eb1a-308">Post-decrement</span></span> |
|                                  | `new T(...)`      | <span data-ttu-id="7eb1a-309">Object and delegate creation</span><span class="sxs-lookup"><span data-stu-id="7eb1a-309">Object and delegate creation</span></span> |
|                                  | `new T(...){...}` | <span data-ttu-id="7eb1a-310">Object creation with initializer</span><span class="sxs-lookup"><span data-stu-id="7eb1a-310">Object creation with initializer</span></span> |
|                                  | `new {...}`       | <span data-ttu-id="7eb1a-311">Anonymous object initializer</span><span class="sxs-lookup"><span data-stu-id="7eb1a-311">Anonymous object initializer</span></span> |
|                                  | `new T[...]`      | <span data-ttu-id="7eb1a-312">Array creation</span><span class="sxs-lookup"><span data-stu-id="7eb1a-312">Array creation</span></span> |
|                                  | `typeof(T)`       | <span data-ttu-id="7eb1a-313">Obtain `System.Type` object for `T`</span><span class="sxs-lookup"><span data-stu-id="7eb1a-313">Obtain `System.Type` object for `T`</span></span> |
|                                  | `checked(x)`      | <span data-ttu-id="7eb1a-314">Evaluate expression in checked context</span><span class="sxs-lookup"><span data-stu-id="7eb1a-314">Evaluate expression in checked context</span></span> |
|                                  | `unchecked(x)`    | <span data-ttu-id="7eb1a-315">Evaluate expression in unchecked context</span><span class="sxs-lookup"><span data-stu-id="7eb1a-315">Evaluate expression in unchecked context</span></span> |
|                                  | `default(T)`      | <span data-ttu-id="7eb1a-316">Obtain default value of type `T`</span><span class="sxs-lookup"><span data-stu-id="7eb1a-316">Obtain default value of type `T`</span></span> |
|                                  | `delegate {...}`  | <span data-ttu-id="7eb1a-317">Anonymous function (anonymous method)</span><span class="sxs-lookup"><span data-stu-id="7eb1a-317">Anonymous function (anonymous method)</span></span> |
| <span data-ttu-id="7eb1a-318">Unary</span><span class="sxs-lookup"><span data-stu-id="7eb1a-318">Unary</span></span>                            | `+x`              | <span data-ttu-id="7eb1a-319">Identity</span><span class="sxs-lookup"><span data-stu-id="7eb1a-319">Identity</span></span> |
|                                  | `-x`              | <span data-ttu-id="7eb1a-320">Negation</span><span class="sxs-lookup"><span data-stu-id="7eb1a-320">Negation</span></span> |
|                                  | `!x`              | <span data-ttu-id="7eb1a-321">Logical negation</span><span class="sxs-lookup"><span data-stu-id="7eb1a-321">Logical negation</span></span> |
|                                  | `~x`              | <span data-ttu-id="7eb1a-322">Bitwise negation</span><span class="sxs-lookup"><span data-stu-id="7eb1a-322">Bitwise negation</span></span> |
|                                  | `++x`             | <span data-ttu-id="7eb1a-323">Pre-increment</span><span class="sxs-lookup"><span data-stu-id="7eb1a-323">Pre-increment</span></span> |
|                                  | `--x`             | <span data-ttu-id="7eb1a-324">Pre-decrement</span><span class="sxs-lookup"><span data-stu-id="7eb1a-324">Pre-decrement</span></span> |
|                                  | `(T)x`            | <span data-ttu-id="7eb1a-325">Explicitly convert `x` to type `T`</span><span class="sxs-lookup"><span data-stu-id="7eb1a-325">Explicitly convert `x` to type `T`</span></span> |
|                                  | `await x`         | <span data-ttu-id="7eb1a-326">Asynchronously wait for `x` to complete</span><span class="sxs-lookup"><span data-stu-id="7eb1a-326">Asynchronously wait for `x` to complete</span></span> |
| <span data-ttu-id="7eb1a-327">Multiplicative</span><span class="sxs-lookup"><span data-stu-id="7eb1a-327">Multiplicative</span></span>                   | `x * y`           | <span data-ttu-id="7eb1a-328">Multiplication</span><span class="sxs-lookup"><span data-stu-id="7eb1a-328">Multiplication</span></span> |
|                                  | `x / y`           | <span data-ttu-id="7eb1a-329">Division</span><span class="sxs-lookup"><span data-stu-id="7eb1a-329">Division</span></span> |
|                                  | `x % y`           | <span data-ttu-id="7eb1a-330">Remainder</span><span class="sxs-lookup"><span data-stu-id="7eb1a-330">Remainder</span></span> |
| <span data-ttu-id="7eb1a-331">Additive</span><span class="sxs-lookup"><span data-stu-id="7eb1a-331">Additive</span></span>                         | `x + y`           | <span data-ttu-id="7eb1a-332">Addition, string concatenation, delegate combination</span><span class="sxs-lookup"><span data-stu-id="7eb1a-332">Addition, string concatenation, delegate combination</span></span> |
|                                  | `x - y`           | <span data-ttu-id="7eb1a-333">Subtraction, delegate removal</span><span class="sxs-lookup"><span data-stu-id="7eb1a-333">Subtraction, delegate removal</span></span> |
| <span data-ttu-id="7eb1a-334">Shift</span><span class="sxs-lookup"><span data-stu-id="7eb1a-334">Shift</span></span>                            | `x << y`          | <span data-ttu-id="7eb1a-335">Shift left</span><span class="sxs-lookup"><span data-stu-id="7eb1a-335">Shift left</span></span> |
|                                  | `x >> y`          | <span data-ttu-id="7eb1a-336">Shift right</span><span class="sxs-lookup"><span data-stu-id="7eb1a-336">Shift right</span></span> |
| <span data-ttu-id="7eb1a-337">Relational and type testing</span><span class="sxs-lookup"><span data-stu-id="7eb1a-337">Relational and type testing</span></span>      | `x < y`           | <span data-ttu-id="7eb1a-338">Less than</span><span class="sxs-lookup"><span data-stu-id="7eb1a-338">Less than</span></span> |
|                                  | `x > y`           | <span data-ttu-id="7eb1a-339">Greater than</span><span class="sxs-lookup"><span data-stu-id="7eb1a-339">Greater than</span></span> |
|                                  | `x <= y`          | <span data-ttu-id="7eb1a-340">Less than or equal</span><span class="sxs-lookup"><span data-stu-id="7eb1a-340">Less than or equal</span></span> |
|                                  | `x >= y`          | <span data-ttu-id="7eb1a-341">Greater than or equal</span><span class="sxs-lookup"><span data-stu-id="7eb1a-341">Greater than or equal</span></span> |
|                                  | `x is T`          | <span data-ttu-id="7eb1a-342">Return `true` if `x` is a `T`, `false` otherwise</span><span class="sxs-lookup"><span data-stu-id="7eb1a-342">Return `true` if `x` is a `T`, `false` otherwise</span></span> |
|                                  | `x as T`          | <span data-ttu-id="7eb1a-343">Return `x` typed as `T`, or `null` if `x` is not a `T`</span><span class="sxs-lookup"><span data-stu-id="7eb1a-343">Return `x` typed as `T`, or `null` if `x` is not a `T`</span></span> |
| <span data-ttu-id="7eb1a-344">Equality</span><span class="sxs-lookup"><span data-stu-id="7eb1a-344">Equality</span></span>                         | `x == y`          | <span data-ttu-id="7eb1a-345">Equal</span><span class="sxs-lookup"><span data-stu-id="7eb1a-345">Equal</span></span>      |
|                                  | `x != y`          | <span data-ttu-id="7eb1a-346">Not equal</span><span class="sxs-lookup"><span data-stu-id="7eb1a-346">Not equal</span></span> |
| <span data-ttu-id="7eb1a-347">Logical AND</span><span class="sxs-lookup"><span data-stu-id="7eb1a-347">Logical AND</span></span>                      | `x & y`           | <span data-ttu-id="7eb1a-348">Integer bitwise AND, boolean logical AND</span><span class="sxs-lookup"><span data-stu-id="7eb1a-348">Integer bitwise AND, boolean logical AND</span></span> |
| <span data-ttu-id="7eb1a-349">Logical XOR</span><span class="sxs-lookup"><span data-stu-id="7eb1a-349">Logical XOR</span></span>                      | `x ^ y`           | <span data-ttu-id="7eb1a-350">Integer bitwise XOR, boolean logical XOR</span><span class="sxs-lookup"><span data-stu-id="7eb1a-350">Integer bitwise XOR, boolean logical XOR</span></span> |
| <span data-ttu-id="7eb1a-351">Logical OR</span><span class="sxs-lookup"><span data-stu-id="7eb1a-351">Logical OR</span></span>                       | <code>x &#124; y</code> | <span data-ttu-id="7eb1a-352">Integer bitwise OR, boolean logical OR</span><span class="sxs-lookup"><span data-stu-id="7eb1a-352">Integer bitwise OR, boolean logical OR</span></span> |
| <span data-ttu-id="7eb1a-353">Conditional AND</span><span class="sxs-lookup"><span data-stu-id="7eb1a-353">Conditional AND</span></span>                  | `x && y`          | <span data-ttu-id="7eb1a-354">Evaluates `y` only if `x` is `true`</span><span class="sxs-lookup"><span data-stu-id="7eb1a-354">Evaluates `y` only if `x` is `true`</span></span> |
| <span data-ttu-id="7eb1a-355">Conditional OR</span><span class="sxs-lookup"><span data-stu-id="7eb1a-355">Conditional OR</span></span>                   | <code>x &#124;&#124; y</code> | <span data-ttu-id="7eb1a-356">Evaluates `y` only if `x` is `false`</span><span class="sxs-lookup"><span data-stu-id="7eb1a-356">Evaluates `y` only if `x` is `false`</span></span> |
| <span data-ttu-id="7eb1a-357">Null coalescing</span><span class="sxs-lookup"><span data-stu-id="7eb1a-357">Null coalescing</span></span>                  | `X ?? y`          | <span data-ttu-id="7eb1a-358">Evaluates to `y` if `x` is `null`, to `x` otherwise</span><span class="sxs-lookup"><span data-stu-id="7eb1a-358">Evaluates to `y` if `x` is `null`, to `x` otherwise</span></span> |
| <span data-ttu-id="7eb1a-359">Conditional</span><span class="sxs-lookup"><span data-stu-id="7eb1a-359">Conditional</span></span>                      | `x ? y : z`       | <span data-ttu-id="7eb1a-360">Evaluates `y` if `x` is `true`, `z` if `x` is `false`</span><span class="sxs-lookup"><span data-stu-id="7eb1a-360">Evaluates `y` if `x` is `true`, `z` if `x` is `false`</span></span> |
| <span data-ttu-id="7eb1a-361">Assignment or anonymous function</span><span class="sxs-lookup"><span data-stu-id="7eb1a-361">Assignment or anonymous function</span></span> | `x = y`           | <span data-ttu-id="7eb1a-362">Assignment</span><span class="sxs-lookup"><span data-stu-id="7eb1a-362">Assignment</span></span> |
|                                  | `x op= y`         | <span data-ttu-id="7eb1a-363">Compound assignment; supported operators are `*=` `/=` `%=` `+=` `-=` `<<=` `>>=` `&=` `^=` <code>&#124;=</code></span><span class="sxs-lookup"><span data-stu-id="7eb1a-363">Compound assignment; supported operators are `*=` `/=` `%=` `+=` `-=` `<<=` `>>=` `&=` `^=` <code>&#124;=</code></span></span> |
|                                  | `(T x) => y`      | <span data-ttu-id="7eb1a-364">Anonymous function (lambda expression)</span><span class="sxs-lookup"><span data-stu-id="7eb1a-364">Anonymous function (lambda expression)</span></span> |

## <a name="statements"></a><span data-ttu-id="7eb1a-365">Statements</span><span class="sxs-lookup"><span data-stu-id="7eb1a-365">Statements</span></span>

<span data-ttu-id="7eb1a-366">The actions of a program are expressed using ***statements***.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-366">The actions of a program are expressed using ***statements***.</span></span> <span data-ttu-id="7eb1a-367">C# supports several different kinds of statements, a number of which are defined in terms of embedded statements.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-367">C# supports several different kinds of statements, a number of which are defined in terms of embedded statements.</span></span>

<span data-ttu-id="7eb1a-368">A ***block*** permits multiple statements to be written in contexts where a single statement is allowed.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-368">A ***block*** permits multiple statements to be written in contexts where a single statement is allowed.</span></span> <span data-ttu-id="7eb1a-369">A block consists of a list of statements written between the delimiters `{` and `}`.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-369">A block consists of a list of statements written between the delimiters `{` and `}`.</span></span>

<span data-ttu-id="7eb1a-370">***Declaration statements*** are used to declare local variables and constants.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-370">***Declaration statements*** are used to declare local variables and constants.</span></span>

<span data-ttu-id="7eb1a-371">***Expression statements*** are used to evaluate expressions.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-371">***Expression statements*** are used to evaluate expressions.</span></span> <span data-ttu-id="7eb1a-372">Expressions that can be used as statements include method invocations, object allocations using the `new` operator, assignments using `=` and the compound assignment operators, increment and decrement operations using the `++` and `--` operators and await expressions.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-372">Expressions that can be used as statements include method invocations, object allocations using the `new` operator, assignments using `=` and the compound assignment operators, increment and decrement operations using the `++` and `--` operators and await expressions.</span></span>

<span data-ttu-id="7eb1a-373">***Selection statements*** are used to select one of a number of possible statements for execution based on the value of some expression.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-373">***Selection statements*** are used to select one of a number of possible statements for execution based on the value of some expression.</span></span> <span data-ttu-id="7eb1a-374">In this group are the `if` and `switch` statements.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-374">In this group are the `if` and `switch` statements.</span></span>

<span data-ttu-id="7eb1a-375">***Iteration statements*** are used to repeatedly execute an embedded statement.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-375">***Iteration statements*** are used to repeatedly execute an embedded statement.</span></span> <span data-ttu-id="7eb1a-376">In this group are the `while`, `do`, `for`, and `foreach` statements.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-376">In this group are the `while`, `do`, `for`, and `foreach` statements.</span></span>

<span data-ttu-id="7eb1a-377">***Jump statements*** are used to transfer control.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-377">***Jump statements*** are used to transfer control.</span></span> <span data-ttu-id="7eb1a-378">In this group are the `break`, `continue`, `goto`, `throw`, `return`, and `yield` statements.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-378">In this group are the `break`, `continue`, `goto`, `throw`, `return`, and `yield` statements.</span></span>

<span data-ttu-id="7eb1a-379">The `try`...`catch` statement is used to catch exceptions that occur during execution of a block, and the `try`...`finally` statement is used to specify finalization code that is always executed, whether an exception occurred or not.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-379">The `try`...`catch` statement is used to catch exceptions that occur during execution of a block, and the `try`...`finally` statement is used to specify finalization code that is always executed, whether an exception occurred or not.</span></span>

<span data-ttu-id="7eb1a-380">The `checked` and `unchecked` statements are used to control the overflow checking context for integral-type arithmetic operations and conversions.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-380">The `checked` and `unchecked` statements are used to control the overflow checking context for integral-type arithmetic operations and conversions.</span></span>

<span data-ttu-id="7eb1a-381">The `lock` statement is used to obtain the mutual-exclusion lock for a given object, execute a statement, and then release the lock.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-381">The `lock` statement is used to obtain the mutual-exclusion lock for a given object, execute a statement, and then release the lock.</span></span>

<span data-ttu-id="7eb1a-382">The `using` statement is used to obtain a resource, execute a statement, and then dispose of that resource.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-382">The `using` statement is used to obtain a resource, execute a statement, and then dispose of that resource.</span></span>

<span data-ttu-id="7eb1a-383">Below are examples of each kind of statement</span><span class="sxs-lookup"><span data-stu-id="7eb1a-383">Below are examples of each kind of statement</span></span>

<span data-ttu-id="7eb1a-384">__Local variable declarations__</span><span class="sxs-lookup"><span data-stu-id="7eb1a-384">__Local variable declarations__</span></span>

```csharp
static void Main() {
   int a;
   int b = 2, c = 3;
   a = 1;
   Console.WriteLine(a + b + c);
}
```


<span data-ttu-id="7eb1a-385">__Local constant declaration__</span><span class="sxs-lookup"><span data-stu-id="7eb1a-385">__Local constant declaration__</span></span>

```csharp
static void Main() {
    const float pi = 3.1415927f;
    const int r = 25;
    Console.WriteLine(pi * r * r);
}
```


<span data-ttu-id="7eb1a-386">__Expression statement__</span><span class="sxs-lookup"><span data-stu-id="7eb1a-386">__Expression statement__</span></span>

```csharp
static void Main() {
    int i;
    i = 123;                // Expression statement
    Console.WriteLine(i);   // Expression statement
    i++;                    // Expression statement
    Console.WriteLine(i);   // Expression statement
}
```

<span data-ttu-id="7eb1a-387">__`if` statement__</span><span class="sxs-lookup"><span data-stu-id="7eb1a-387">__`if` statement__</span></span>

```csharp
static void Main(string[] args) {
    if (args.Length == 0) {
        Console.WriteLine("No arguments");
    }
    else {
        Console.WriteLine("One or more arguments");
    }
}
```


<span data-ttu-id="7eb1a-388">__`switch` statement__</span><span class="sxs-lookup"><span data-stu-id="7eb1a-388">__`switch` statement__</span></span>

```csharp
static void Main(string[] args) {
    int n = args.Length;
    switch (n) {
        case 0:
            Console.WriteLine("No arguments");
            break;
        case 1:
            Console.WriteLine("One argument");
            break;
        default:
            Console.WriteLine("{0} arguments", n);
            break;
    }
}
```

<span data-ttu-id="7eb1a-389">__`while` statement__</span><span class="sxs-lookup"><span data-stu-id="7eb1a-389">__`while` statement__</span></span>

```csharp
static void Main(string[] args) {
    int i = 0;
    while (i < args.Length) {
        Console.WriteLine(args[i]);
        i++;
    }
}
```


<span data-ttu-id="7eb1a-390">__`do` statement__</span><span class="sxs-lookup"><span data-stu-id="7eb1a-390">__`do` statement__</span></span>

```csharp
static void Main() {
    string s;
    do {
        s = Console.ReadLine();
        if (s != null) Console.WriteLine(s);
    } while (s != null);
}
```

<span data-ttu-id="7eb1a-391">__`for` statement__</span><span class="sxs-lookup"><span data-stu-id="7eb1a-391">__`for` statement__</span></span>

```csharp
static void Main(string[] args) {
    for (int i = 0; i < args.Length; i++) {
        Console.WriteLine(args[i]);
    }
}
```

<span data-ttu-id="7eb1a-392">__`foreach` statement__</span><span class="sxs-lookup"><span data-stu-id="7eb1a-392">__`foreach` statement__</span></span>

```csharp
static void Main(string[] args) {
    foreach (string s in args) {
        Console.WriteLine(s);
    }
}
```

<span data-ttu-id="7eb1a-393">__`break` statement__</span><span class="sxs-lookup"><span data-stu-id="7eb1a-393">__`break` statement__</span></span>

```csharp
static void Main() {
    while (true) {
        string s = Console.ReadLine();
        if (s == null) break;
        Console.WriteLine(s);
    }
}
```

<span data-ttu-id="7eb1a-394">__`continue` statement__</span><span class="sxs-lookup"><span data-stu-id="7eb1a-394">__`continue` statement__</span></span>

```csharp
static void Main(string[] args) {
    for (int i = 0; i < args.Length; i++) {
        if (args[i].StartsWith("/")) continue;
        Console.WriteLine(args[i]);
    }
}
```

<span data-ttu-id="7eb1a-395">__`goto` statement__</span><span class="sxs-lookup"><span data-stu-id="7eb1a-395">__`goto` statement__</span></span>

```csharp
static void Main(string[] args) {
    int i = 0;
    goto check;
    loop:
    Console.WriteLine(args[i++]);
    check:
    if (i < args.Length) goto loop;
}
```

<span data-ttu-id="7eb1a-396">__`return` statement__</span><span class="sxs-lookup"><span data-stu-id="7eb1a-396">__`return` statement__</span></span>

```csharp
static int Add(int a, int b) {
    return a + b;
}

static void Main() {
    Console.WriteLine(Add(1, 2));
    return;
}
```

<span data-ttu-id="7eb1a-397">__`yield` statement__</span><span class="sxs-lookup"><span data-stu-id="7eb1a-397">__`yield` statement__</span></span>

```csharp
static IEnumerable<int> Range(int from, int to) {
    for (int i = from; i < to; i++) {
        yield return i;
    }
    yield break;
}

static void Main() {
    foreach (int x in Range(-10,10)) {
        Console.WriteLine(x);
    }
}
```

<span data-ttu-id="7eb1a-398">__`throw` and `try` statements__</span><span class="sxs-lookup"><span data-stu-id="7eb1a-398">__`throw` and `try` statements__</span></span>

```csharp
static double Divide(double x, double y) {
    if (y == 0) throw new DivideByZeroException();
    return x / y;
}

static void Main(string[] args) {
    try {
        if (args.Length != 2) {
            throw new Exception("Two numbers required");
        }
        double x = double.Parse(args[0]);
        double y = double.Parse(args[1]);
        Console.WriteLine(Divide(x, y));
    }
    catch (Exception e) {
        Console.WriteLine(e.Message);
    }
    finally {
        Console.WriteLine("Good bye!");
    }
}
```

<span data-ttu-id="7eb1a-399">__`checked` and `unchecked` statements__</span><span class="sxs-lookup"><span data-stu-id="7eb1a-399">__`checked` and `unchecked` statements__</span></span>

```csharp
static void Main() {
    int i = int.MaxValue;
    checked {
        Console.WriteLine(i + 1);        // Exception
    }
    unchecked {
        Console.WriteLine(i + 1);        // Overflow
    }
}
```

<span data-ttu-id="7eb1a-400">__`lock` statement__</span><span class="sxs-lookup"><span data-stu-id="7eb1a-400">__`lock` statement__</span></span>

```csharp
class Account
{
    decimal balance;
    public void Withdraw(decimal amount) {
        lock (this) {
            if (amount > balance) {
                throw new Exception("Insufficient funds");
            }
            balance -= amount;
        }
    }
}
```

<span data-ttu-id="7eb1a-401">__`using` statement__</span><span class="sxs-lookup"><span data-stu-id="7eb1a-401">__`using` statement__</span></span>

```csharp
static void Main() {
    using (TextWriter w = File.CreateText("test.txt")) {
        w.WriteLine("Line one");
        w.WriteLine("Line two");
        w.WriteLine("Line three");
    }
}
```

## <a name="classes-and-objects"></a><span data-ttu-id="7eb1a-402">Classes and objects</span><span class="sxs-lookup"><span data-stu-id="7eb1a-402">Classes and objects</span></span>

<span data-ttu-id="7eb1a-403">***Classes*** are the most fundamental of C#'s types.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-403">***Classes*** are the most fundamental of C#'s types.</span></span> <span data-ttu-id="7eb1a-404">A class is a data structure that combines state (fields) and actions (methods and other function members) in a single unit.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-404">A class is a data structure that combines state (fields) and actions (methods and other function members) in a single unit.</span></span> <span data-ttu-id="7eb1a-405">A class provides a definition for dynamically created ***instances*** of the class, also known as ***objects***.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-405">A class provides a definition for dynamically created ***instances*** of the class, also known as ***objects***.</span></span> <span data-ttu-id="7eb1a-406">Classes support ***inheritance*** and ***polymorphism***, mechanisms whereby ***derived classes*** can extend and specialize ***base classes***.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-406">Classes support ***inheritance*** and ***polymorphism***, mechanisms whereby ***derived classes*** can extend and specialize ***base classes***.</span></span>

<span data-ttu-id="7eb1a-407">New classes are created using class declarations.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-407">New classes are created using class declarations.</span></span> <span data-ttu-id="7eb1a-408">A class declaration starts with a header that specifies the attributes and modifiers of the class, the name of the class, the base class (if given), and the interfaces implemented by the class.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-408">A class declaration starts with a header that specifies the attributes and modifiers of the class, the name of the class, the base class (if given), and the interfaces implemented by the class.</span></span> <span data-ttu-id="7eb1a-409">The header is followed by the class body, which consists of a list of member declarations written between the delimiters `{` and `}`.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-409">The header is followed by the class body, which consists of a list of member declarations written between the delimiters `{` and `}`.</span></span>

<span data-ttu-id="7eb1a-410">The following is a declaration of a simple class named `Point`:</span><span class="sxs-lookup"><span data-stu-id="7eb1a-410">The following is a declaration of a simple class named `Point`:</span></span>

```csharp
public class Point
{
    public int x, y;

    public Point(int x, int y) {
        this.x = x;
        this.y = y;
    }
}
```
<span data-ttu-id="7eb1a-411">Instances of classes are created using the `new` operator, which allocates memory for a new instance, invokes a constructor to initialize the instance, and returns a reference to the instance.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-411">Instances of classes are created using the `new` operator, which allocates memory for a new instance, invokes a constructor to initialize the instance, and returns a reference to the instance.</span></span> <span data-ttu-id="7eb1a-412">The following statements create two `Point` objects and store references to those objects in two variables:</span><span class="sxs-lookup"><span data-stu-id="7eb1a-412">The following statements create two `Point` objects and store references to those objects in two variables:</span></span>

```
Point p1 = new Point(0, 0);
Point p2 = new Point(10, 20);
```
<span data-ttu-id="7eb1a-413">The memory occupied by an object is automatically reclaimed when the object is no longer in use.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-413">The memory occupied by an object is automatically reclaimed when the object is no longer in use.</span></span> <span data-ttu-id="7eb1a-414">It is neither necessary nor possible to explicitly deallocate objects in C#.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-414">It is neither necessary nor possible to explicitly deallocate objects in C#.</span></span>

### <a name="members"></a><span data-ttu-id="7eb1a-415">Members</span><span class="sxs-lookup"><span data-stu-id="7eb1a-415">Members</span></span>

<span data-ttu-id="7eb1a-416">The members of a class are either ***static members*** or ***instance members***.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-416">The members of a class are either ***static members*** or ***instance members***.</span></span> <span data-ttu-id="7eb1a-417">Static members belong to classes, and instance members belong to objects (instances of classes).</span><span class="sxs-lookup"><span data-stu-id="7eb1a-417">Static members belong to classes, and instance members belong to objects (instances of classes).</span></span>

<span data-ttu-id="7eb1a-418">The following table provides an overview of the kinds of members a class can contain.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-418">The following table provides an overview of the kinds of members a class can contain.</span></span>


| <span data-ttu-id="7eb1a-419">__Member__</span><span class="sxs-lookup"><span data-stu-id="7eb1a-419">__Member__</span></span>   | <span data-ttu-id="7eb1a-420">__Description__</span><span class="sxs-lookup"><span data-stu-id="7eb1a-420">__Description__</span></span> |
|------------  |-----------------|
| <span data-ttu-id="7eb1a-421">Constants</span><span class="sxs-lookup"><span data-stu-id="7eb1a-421">Constants</span></span>    | <span data-ttu-id="7eb1a-422">Constant values associated with the class</span><span class="sxs-lookup"><span data-stu-id="7eb1a-422">Constant values associated with the class</span></span> |
| <span data-ttu-id="7eb1a-423">Fields</span><span class="sxs-lookup"><span data-stu-id="7eb1a-423">Fields</span></span>       | <span data-ttu-id="7eb1a-424">Variables of the class</span><span class="sxs-lookup"><span data-stu-id="7eb1a-424">Variables of the class</span></span> |
| <span data-ttu-id="7eb1a-425">Methods</span><span class="sxs-lookup"><span data-stu-id="7eb1a-425">Methods</span></span>      | <span data-ttu-id="7eb1a-426">Computations and actions that can be performed by the class</span><span class="sxs-lookup"><span data-stu-id="7eb1a-426">Computations and actions that can be performed by the class</span></span> |
| <span data-ttu-id="7eb1a-427">Properties</span><span class="sxs-lookup"><span data-stu-id="7eb1a-427">Properties</span></span>   | <span data-ttu-id="7eb1a-428">Actions associated with reading and writing named properties of the class</span><span class="sxs-lookup"><span data-stu-id="7eb1a-428">Actions associated with reading and writing named properties of the class</span></span> |
| <span data-ttu-id="7eb1a-429">Indexers</span><span class="sxs-lookup"><span data-stu-id="7eb1a-429">Indexers</span></span>     | <span data-ttu-id="7eb1a-430">Actions associated with indexing instances of the class like an array</span><span class="sxs-lookup"><span data-stu-id="7eb1a-430">Actions associated with indexing instances of the class like an array</span></span> |
| <span data-ttu-id="7eb1a-431">Events</span><span class="sxs-lookup"><span data-stu-id="7eb1a-431">Events</span></span>       | <span data-ttu-id="7eb1a-432">Notifications that can be generated by the class</span><span class="sxs-lookup"><span data-stu-id="7eb1a-432">Notifications that can be generated by the class</span></span> |
| <span data-ttu-id="7eb1a-433">Operators</span><span class="sxs-lookup"><span data-stu-id="7eb1a-433">Operators</span></span>    | <span data-ttu-id="7eb1a-434">Conversions and expression operators supported by the class</span><span class="sxs-lookup"><span data-stu-id="7eb1a-434">Conversions and expression operators supported by the class</span></span> |
| <span data-ttu-id="7eb1a-435">Constructors</span><span class="sxs-lookup"><span data-stu-id="7eb1a-435">Constructors</span></span> | <span data-ttu-id="7eb1a-436">Actions required to initialize instances of the class or the class itself</span><span class="sxs-lookup"><span data-stu-id="7eb1a-436">Actions required to initialize instances of the class or the class itself</span></span> |
| <span data-ttu-id="7eb1a-437">Destructors</span><span class="sxs-lookup"><span data-stu-id="7eb1a-437">Destructors</span></span>  | <span data-ttu-id="7eb1a-438">Actions to perform before instances of the class are permanently discarded</span><span class="sxs-lookup"><span data-stu-id="7eb1a-438">Actions to perform before instances of the class are permanently discarded</span></span> |
| <span data-ttu-id="7eb1a-439">Types</span><span class="sxs-lookup"><span data-stu-id="7eb1a-439">Types</span></span>        | <span data-ttu-id="7eb1a-440">Nested types declared by the class</span><span class="sxs-lookup"><span data-stu-id="7eb1a-440">Nested types declared by the class</span></span> |

### <a name="accessibility"></a><span data-ttu-id="7eb1a-441">Accessibility</span><span class="sxs-lookup"><span data-stu-id="7eb1a-441">Accessibility</span></span>

<span data-ttu-id="7eb1a-442">Each member of a class has an associated accessibility, which controls the regions of program text that are able to access the member.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-442">Each member of a class has an associated accessibility, which controls the regions of program text that are able to access the member.</span></span> <span data-ttu-id="7eb1a-443">There are five possible forms of accessibility.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-443">There are five possible forms of accessibility.</span></span> <span data-ttu-id="7eb1a-444">These are summarized in the following table.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-444">These are summarized in the following table.</span></span>


| <span data-ttu-id="7eb1a-445">__Accessibility__</span><span class="sxs-lookup"><span data-stu-id="7eb1a-445">__Accessibility__</span></span>    | <span data-ttu-id="7eb1a-446">__Meaning__</span><span class="sxs-lookup"><span data-stu-id="7eb1a-446">__Meaning__</span></span> |
|----------------------|-----------------|
| `public`             | <span data-ttu-id="7eb1a-447">Access not limited</span><span class="sxs-lookup"><span data-stu-id="7eb1a-447">Access not limited</span></span> |
| `protected`          | <span data-ttu-id="7eb1a-448">Access limited to this class or classes derived from this class</span><span class="sxs-lookup"><span data-stu-id="7eb1a-448">Access limited to this class or classes derived from this class</span></span> |
| `internal`           | <span data-ttu-id="7eb1a-449">Access limited to this program</span><span class="sxs-lookup"><span data-stu-id="7eb1a-449">Access limited to this program</span></span> |
| `protected internal` | <span data-ttu-id="7eb1a-450">Access limited to this program or classes derived from this class</span><span class="sxs-lookup"><span data-stu-id="7eb1a-450">Access limited to this program or classes derived from this class</span></span> |
| `private`            | <span data-ttu-id="7eb1a-451">Access limited to this class</span><span class="sxs-lookup"><span data-stu-id="7eb1a-451">Access limited to this class</span></span> |

### <a name="type-parameters"></a><span data-ttu-id="7eb1a-452">Type parameters</span><span class="sxs-lookup"><span data-stu-id="7eb1a-452">Type parameters</span></span>

<span data-ttu-id="7eb1a-453">A class definition may specify a set of type parameters by following the class name with angle brackets enclosing a list of type parameter names.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-453">A class definition may specify a set of type parameters by following the class name with angle brackets enclosing a list of type parameter names.</span></span> <span data-ttu-id="7eb1a-454">The type parameters can the be used in the body of the class declarations to define the members of the class.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-454">The type parameters can the be used in the body of the class declarations to define the members of the class.</span></span> <span data-ttu-id="7eb1a-455">In the following example, the type parameters of `Pair` are `TFirst` and `TSecond`:</span><span class="sxs-lookup"><span data-stu-id="7eb1a-455">In the following example, the type parameters of `Pair` are `TFirst` and `TSecond`:</span></span>

```csharp
public class Pair<TFirst,TSecond>
{
    public TFirst First;
    public TSecond Second;
}
```
<span data-ttu-id="7eb1a-456">A class type that is declared to take type parameters is called a generic class type.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-456">A class type that is declared to take type parameters is called a generic class type.</span></span> <span data-ttu-id="7eb1a-457">Struct, interface and delegate types can also be generic.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-457">Struct, interface and delegate types can also be generic.</span></span>

<span data-ttu-id="7eb1a-458">When the generic class is used, type arguments must be provided for each of the type parameters:</span><span class="sxs-lookup"><span data-stu-id="7eb1a-458">When the generic class is used, type arguments must be provided for each of the type parameters:</span></span>

```csharp
Pair<int,string> pair = new Pair<int,string> { First = 1, Second = "two" };
int i = pair.First;     // TFirst is int
string s = pair.Second; // TSecond is string
```
<span data-ttu-id="7eb1a-459">A generic type with type arguments provided, like `Pair<int,string>
    ` above, is called a constructed type.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-459">A generic type with type arguments provided, like `Pair<int,string>
    ` above, is called a constructed type.</span></span>

### <a name="base-classes"></a><span data-ttu-id="7eb1a-460">Base classes</span><span class="sxs-lookup"><span data-stu-id="7eb1a-460">Base classes</span></span>

<span data-ttu-id="7eb1a-461">A class declaration may specify a base class by following the class name and type parameters with a colon and the name of the base class.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-461">A class declaration may specify a base class by following the class name and type parameters with a colon and the name of the base class.</span></span> <span data-ttu-id="7eb1a-462">Omitting a base class specification is the same as deriving from type `object`.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-462">Omitting a base class specification is the same as deriving from type `object`.</span></span> <span data-ttu-id="7eb1a-463">In the following example, the base class of `Point3D` is `Point`, and the base class of `Point` is `object`:</span><span class="sxs-lookup"><span data-stu-id="7eb1a-463">In the following example, the base class of `Point3D` is `Point`, and the base class of `Point` is `object`:</span></span>

```csharp
public class Point
{
    public int x, y;

    public Point(int x, int y) {
        this.x = x;
        this.y = y;
    }
}

public class Point3D: Point
{
    public int z;

    public Point3D(int x, int y, int z): base(x, y) {
        this.z = z;
    }
}
```
<span data-ttu-id="7eb1a-464">A class inherits the members of its base class.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-464">A class inherits the members of its base class.</span></span> <span data-ttu-id="7eb1a-465">Inheritance means that a class implicitly contains all members of its base class, except for the instance and static constructors, and the destructors of the base class.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-465">Inheritance means that a class implicitly contains all members of its base class, except for the instance and static constructors, and the destructors of the base class.</span></span> <span data-ttu-id="7eb1a-466">A derived class can add new members to those it inherits, but it cannot remove the definition of an inherited member.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-466">A derived class can add new members to those it inherits, but it cannot remove the definition of an inherited member.</span></span> <span data-ttu-id="7eb1a-467">In the previous example, `Point3D` inherits the `x` and `y` fields from `Point`, and every `Point3D` instance contains three fields, `x`, `y`, and `z`.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-467">In the previous example, `Point3D` inherits the `x` and `y` fields from `Point`, and every `Point3D` instance contains three fields, `x`, `y`, and `z`.</span></span>

<span data-ttu-id="7eb1a-468">An implicit conversion exists from a class type to any of its base class types.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-468">An implicit conversion exists from a class type to any of its base class types.</span></span> <span data-ttu-id="7eb1a-469">Therefore, a variable of a class type can reference an instance of that class or an instance of any derived class.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-469">Therefore, a variable of a class type can reference an instance of that class or an instance of any derived class.</span></span> <span data-ttu-id="7eb1a-470">For example, given the previous class declarations, a variable of type `Point` can reference either a `Point` or a `Point3D`:</span><span class="sxs-lookup"><span data-stu-id="7eb1a-470">For example, given the previous class declarations, a variable of type `Point` can reference either a `Point` or a `Point3D`:</span></span>

```csharp
Point a = new Point(10, 20);
Point b = new Point3D(10, 20, 30);
```

### <a name="fields"></a><span data-ttu-id="7eb1a-471">Fields</span><span class="sxs-lookup"><span data-stu-id="7eb1a-471">Fields</span></span>

<span data-ttu-id="7eb1a-472">A field is a variable that is associated with a class or with an instance of a class.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-472">A field is a variable that is associated with a class or with an instance of a class.</span></span>

<span data-ttu-id="7eb1a-473">A field declared with the `static` modifier defines a ***static field***.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-473">A field declared with the `static` modifier defines a ***static field***.</span></span> <span data-ttu-id="7eb1a-474">A static field identifies exactly one storage location.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-474">A static field identifies exactly one storage location.</span></span> <span data-ttu-id="7eb1a-475">No matter how many instances of a class are created, there is only ever one copy of a static field.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-475">No matter how many instances of a class are created, there is only ever one copy of a static field.</span></span>

<span data-ttu-id="7eb1a-476">A field declared without the `static` modifier defines an ***instance field***.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-476">A field declared without the `static` modifier defines an ***instance field***.</span></span> <span data-ttu-id="7eb1a-477">Every instance of a class contains a separate copy of all the instance fields of that class.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-477">Every instance of a class contains a separate copy of all the instance fields of that class.</span></span>

<span data-ttu-id="7eb1a-478">In the following example, each instance of the `Color` class has a separate copy of the `r`, `g`, and `b` instance fields, but there is only one copy of the `Black`, `White`, `Red`, `Green`, and `Blue` static fields:</span><span class="sxs-lookup"><span data-stu-id="7eb1a-478">In the following example, each instance of the `Color` class has a separate copy of the `r`, `g`, and `b` instance fields, but there is only one copy of the `Black`, `White`, `Red`, `Green`, and `Blue` static fields:</span></span>

```csharp
public class Color
{
    public static readonly Color Black = new Color(0, 0, 0);
    public static readonly Color White = new Color(255, 255, 255);
    public static readonly Color Red = new Color(255, 0, 0);
    public static readonly Color Green = new Color(0, 255, 0);
    public static readonly Color Blue = new Color(0, 0, 255);
    private byte r, g, b;

    public Color(byte r, byte g, byte b) {
        this.r = r;
        this.g = g;
        this.b = b;
    }
}
```
<span data-ttu-id="7eb1a-479">As shown in the previous example, ***read-only fields*** may be declared with a `readonly` modifier.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-479">As shown in the previous example, ***read-only fields*** may be declared with a `readonly` modifier.</span></span> <span data-ttu-id="7eb1a-480">Assignment to a `readonly` field can only occur as part of the field's declaration or in a constructor in the same class.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-480">Assignment to a `readonly` field can only occur as part of the field's declaration or in a constructor in the same class.</span></span>

### <a name="methods"></a><span data-ttu-id="7eb1a-481">Methods</span><span class="sxs-lookup"><span data-stu-id="7eb1a-481">Methods</span></span>

<span data-ttu-id="7eb1a-482">A ***method*** is a member that implements a computation or action that can be performed by an object or class.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-482">A ***method*** is a member that implements a computation or action that can be performed by an object or class.</span></span> <span data-ttu-id="7eb1a-483">***Static methods*** are accessed through the class.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-483">***Static methods*** are accessed through the class.</span></span> <span data-ttu-id="7eb1a-484">***Instance methods*** are accessed through instances of the class.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-484">***Instance methods*** are accessed through instances of the class.</span></span>

<span data-ttu-id="7eb1a-485">Methods have a (possibly empty) list of ***parameters***, which represent values or variable references passed to the method, and a ***return type***, which specifies the type of the value computed and returned by the method.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-485">Methods have a (possibly empty) list of ***parameters***, which represent values or variable references passed to the method, and a ***return type***, which specifies the type of the value computed and returned by the method.</span></span> <span data-ttu-id="7eb1a-486">A method's return type is `void` if it does not return a value.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-486">A method's return type is `void` if it does not return a value.</span></span>

<span data-ttu-id="7eb1a-487">Like types, methods may also have a set of type parameters, for which type arguments must be specified when the method is called.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-487">Like types, methods may also have a set of type parameters, for which type arguments must be specified when the method is called.</span></span> <span data-ttu-id="7eb1a-488">Unlike types, the type arguments can often be inferred from the arguments of a method call and need not be explicitly given.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-488">Unlike types, the type arguments can often be inferred from the arguments of a method call and need not be explicitly given.</span></span>

<span data-ttu-id="7eb1a-489">The ***signature*** of a method must be unique in the class in which the method is declared.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-489">The ***signature*** of a method must be unique in the class in which the method is declared.</span></span> <span data-ttu-id="7eb1a-490">The signature of a method consists of the name of the method, the number of type parameters and the number, modifiers, and types of its parameters.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-490">The signature of a method consists of the name of the method, the number of type parameters and the number, modifiers, and types of its parameters.</span></span> <span data-ttu-id="7eb1a-491">The signature of a method does not include the return type.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-491">The signature of a method does not include the return type.</span></span>

#### <a name="parameters"></a><span data-ttu-id="7eb1a-492">Parameters</span><span class="sxs-lookup"><span data-stu-id="7eb1a-492">Parameters</span></span>

<span data-ttu-id="7eb1a-493">Parameters are used to pass values or variable references to methods.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-493">Parameters are used to pass values or variable references to methods.</span></span> <span data-ttu-id="7eb1a-494">The parameters of a method get their actual values from the ***arguments*** that are specified when the method is invoked.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-494">The parameters of a method get their actual values from the ***arguments*** that are specified when the method is invoked.</span></span> <span data-ttu-id="7eb1a-495">There are four kinds of parameters: value parameters, reference parameters, output parameters, and parameter arrays.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-495">There are four kinds of parameters: value parameters, reference parameters, output parameters, and parameter arrays.</span></span>

<span data-ttu-id="7eb1a-496">A ***value parameter*** is used for input parameter passing.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-496">A ***value parameter*** is used for input parameter passing.</span></span> <span data-ttu-id="7eb1a-497">A value parameter corresponds to a local variable that gets its initial value from the argument that was passed for the parameter.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-497">A value parameter corresponds to a local variable that gets its initial value from the argument that was passed for the parameter.</span></span> <span data-ttu-id="7eb1a-498">Modifications to a value parameter do not affect the argument that was passed for the parameter.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-498">Modifications to a value parameter do not affect the argument that was passed for the parameter.</span></span>

<span data-ttu-id="7eb1a-499">Value parameters can be optional, by specifying a default value so that corresponding arguments can be omitted.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-499">Value parameters can be optional, by specifying a default value so that corresponding arguments can be omitted.</span></span>

<span data-ttu-id="7eb1a-500">A ***reference parameter*** is used for both input and output parameter passing.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-500">A ***reference parameter*** is used for both input and output parameter passing.</span></span> <span data-ttu-id="7eb1a-501">The argument passed for a reference parameter must be a variable, and during execution of the method, the reference parameter represents the same storage location as the argument variable.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-501">The argument passed for a reference parameter must be a variable, and during execution of the method, the reference parameter represents the same storage location as the argument variable.</span></span> <span data-ttu-id="7eb1a-502">A reference parameter is declared with the `ref` modifier.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-502">A reference parameter is declared with the `ref` modifier.</span></span> <span data-ttu-id="7eb1a-503">The following example shows the use of `ref` parameters.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-503">The following example shows the use of `ref` parameters.</span></span>

```csharp
using System;

class Test
{
    static void Swap(ref int x, ref int y) {
        int temp = x;
        x = y;
        y = temp;
    }

    static void Main() {
        int i = 1, j = 2;
        Swap(ref i, ref j);
        Console.WriteLine("{0} {1}", i, j);            // Outputs "2 1"
    }
}
```
<span data-ttu-id="7eb1a-504">An ***output parameter*** is used for output parameter passing.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-504">An ***output parameter*** is used for output parameter passing.</span></span> <span data-ttu-id="7eb1a-505">An output parameter is similar to a reference parameter except that the initial value of the caller-provided argument is unimportant.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-505">An output parameter is similar to a reference parameter except that the initial value of the caller-provided argument is unimportant.</span></span> <span data-ttu-id="7eb1a-506">An output parameter is declared with the `out` modifier.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-506">An output parameter is declared with the `out` modifier.</span></span> <span data-ttu-id="7eb1a-507">The following example shows the use of `out` parameters.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-507">The following example shows the use of `out` parameters.</span></span>

```csharp
using System;

class Test
{
    static void Divide(int x, int y, out int result, out int remainder) {
        result = x / y;
        remainder = x % y;
    }

    static void Main() {
        int res, rem;
        Divide(10, 3, out res, out rem);
        Console.WriteLine("{0} {1}", res, rem);    // Outputs "3 1"
    }
}
```
<span data-ttu-id="7eb1a-508">A ***parameter array*** permits a variable number of arguments to be passed to a method.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-508">A ***parameter array*** permits a variable number of arguments to be passed to a method.</span></span> <span data-ttu-id="7eb1a-509">A parameter array is declared with the `params` modifier.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-509">A parameter array is declared with the `params` modifier.</span></span> <span data-ttu-id="7eb1a-510">Only the last parameter of a method can be a parameter array, and the type of a parameter array must be a single-dimensional array type.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-510">Only the last parameter of a method can be a parameter array, and the type of a parameter array must be a single-dimensional array type.</span></span> <span data-ttu-id="7eb1a-511">The `Write` and `WriteLine` methods of the `System.Console` class are good examples of parameter array usage.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-511">The `Write` and `WriteLine` methods of the `System.Console` class are good examples of parameter array usage.</span></span> <span data-ttu-id="7eb1a-512">They are declared as follows.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-512">They are declared as follows.</span></span>

```csharp
public class Console
{
    public static void Write(string fmt, params object[] args) {...}
    public static void WriteLine(string fmt, params object[] args) {...}
    ...
}
```
<span data-ttu-id="7eb1a-513">Within a method that uses a parameter array, the parameter array behaves exactly like a regular parameter of an array type.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-513">Within a method that uses a parameter array, the parameter array behaves exactly like a regular parameter of an array type.</span></span> <span data-ttu-id="7eb1a-514">However, in an invocation of a method with a parameter array, it is possible to pass either a single argument of the parameter array type or any number of arguments of the element type of the parameter array.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-514">However, in an invocation of a method with a parameter array, it is possible to pass either a single argument of the parameter array type or any number of arguments of the element type of the parameter array.</span></span> <span data-ttu-id="7eb1a-515">In the latter case, an array instance is automatically created and initialized with the given arguments.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-515">In the latter case, an array instance is automatically created and initialized with the given arguments.</span></span> <span data-ttu-id="7eb1a-516">This example</span><span class="sxs-lookup"><span data-stu-id="7eb1a-516">This example</span></span>

```csharp
Console.WriteLine("x={0} y={1} z={2}", x, y, z);
```
<span data-ttu-id="7eb1a-517">is equivalent to writing the following.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-517">is equivalent to writing the following.</span></span>

```csharp
string s = "x={0} y={1} z={2}";
object[] args = new object[3];
args[0] = x;
args[1] = y;
args[2] = z;
Console.WriteLine(s, args);
```

#### <a name="method-body-and-local-variables"></a><span data-ttu-id="7eb1a-518">Method body and local variables</span><span class="sxs-lookup"><span data-stu-id="7eb1a-518">Method body and local variables</span></span>

<span data-ttu-id="7eb1a-519">A method's body specifies the statements to execute when the method is invoked.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-519">A method's body specifies the statements to execute when the method is invoked.</span></span>

<span data-ttu-id="7eb1a-520">A method body can declare variables that are specific to the invocation of the method.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-520">A method body can declare variables that are specific to the invocation of the method.</span></span> <span data-ttu-id="7eb1a-521">Such variables are called ***local variables***.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-521">Such variables are called ***local variables***.</span></span> <span data-ttu-id="7eb1a-522">A local variable declaration specifies a type name, a variable name, and possibly an initial value.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-522">A local variable declaration specifies a type name, a variable name, and possibly an initial value.</span></span> <span data-ttu-id="7eb1a-523">The following example declares a local variable `i` with an initial value of zero and a local variable `j` with no initial value.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-523">The following example declares a local variable `i` with an initial value of zero and a local variable `j` with no initial value.</span></span>

```csharp
using System;

class Squares
{
    static void Main() {
        int i = 0;
        int j;
        while (i < 10) {
            j = i * i;
            Console.WriteLine("{0} x {0} = {1}", i, j);
            i = i + 1;
        }
    }
}
```
<span data-ttu-id="7eb1a-524">C# requires a local variable to be ***definitely assigned*** before its value can be obtained.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-524">C# requires a local variable to be ***definitely assigned*** before its value can be obtained.</span></span> <span data-ttu-id="7eb1a-525">For example, if the declaration of the previous `i` did not include an initial value, the compiler would report an error for the subsequent usages of `i` because `i` would not be definitely assigned at those points in the program.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-525">For example, if the declaration of the previous `i` did not include an initial value, the compiler would report an error for the subsequent usages of `i` because `i` would not be definitely assigned at those points in the program.</span></span>

<span data-ttu-id="7eb1a-526">A method can use `return` statements to return control to its caller.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-526">A method can use `return` statements to return control to its caller.</span></span> <span data-ttu-id="7eb1a-527">In a method returning `void`, `return` statements cannot specify an expression.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-527">In a method returning `void`, `return` statements cannot specify an expression.</span></span> <span data-ttu-id="7eb1a-528">In a method returning non-`void`, `return` statements must include an expression that computes the return value.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-528">In a method returning non-`void`, `return` statements must include an expression that computes the return value.</span></span>

#### <a name="static-and-instance-methods"></a><span data-ttu-id="7eb1a-529">Static and instance methods</span><span class="sxs-lookup"><span data-stu-id="7eb1a-529">Static and instance methods</span></span>

<span data-ttu-id="7eb1a-530">A method declared with a `static` modifier is a ***static method***.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-530">A method declared with a `static` modifier is a ***static method***.</span></span> <span data-ttu-id="7eb1a-531">A static method does not operate on a specific instance and can only directly access static members.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-531">A static method does not operate on a specific instance and can only directly access static members.</span></span>

<span data-ttu-id="7eb1a-532">A method declared without a `static` modifier is an ***instance method***.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-532">A method declared without a `static` modifier is an ***instance method***.</span></span> <span data-ttu-id="7eb1a-533">An instance method operates on a specific instance and can access both static and instance members.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-533">An instance method operates on a specific instance and can access both static and instance members.</span></span> <span data-ttu-id="7eb1a-534">The instance on which an instance method was invoked can be explicitly accessed as `this`.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-534">The instance on which an instance method was invoked can be explicitly accessed as `this`.</span></span> <span data-ttu-id="7eb1a-535">It is an error to refer to `this` in a static method.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-535">It is an error to refer to `this` in a static method.</span></span>

<span data-ttu-id="7eb1a-536">The following `Entity` class has both static and instance members.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-536">The following `Entity` class has both static and instance members.</span></span>

```csharp
class Entity
{
    static int nextSerialNo;
    int serialNo;

    public Entity() {
        serialNo = nextSerialNo++;
    }

    public int GetSerialNo() {
        return serialNo;
    }

    public static int GetNextSerialNo() {
        return nextSerialNo;
    }

    public static void SetNextSerialNo(int value) {
        nextSerialNo = value;
    }
}
```
<span data-ttu-id="7eb1a-537">Each `Entity` instance contains a serial number (and presumably some other information that is not shown here).</span><span class="sxs-lookup"><span data-stu-id="7eb1a-537">Each `Entity` instance contains a serial number (and presumably some other information that is not shown here).</span></span> <span data-ttu-id="7eb1a-538">The `Entity` constructor (which is like an instance method) initializes the new instance with the next available serial number.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-538">The `Entity` constructor (which is like an instance method) initializes the new instance with the next available serial number.</span></span> <span data-ttu-id="7eb1a-539">Because the constructor is an instance member, it is permitted to access both the `serialNo` instance field and the `nextSerialNo` static field.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-539">Because the constructor is an instance member, it is permitted to access both the `serialNo` instance field and the `nextSerialNo` static field.</span></span>

<span data-ttu-id="7eb1a-540">The `GetNextSerialNo` and `SetNextSerialNo` static methods can access the `nextSerialNo` static field, but it would be an error for them to directly access the `serialNo` instance field.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-540">The `GetNextSerialNo` and `SetNextSerialNo` static methods can access the `nextSerialNo` static field, but it would be an error for them to directly access the `serialNo` instance field.</span></span>

<span data-ttu-id="7eb1a-541">The following example shows the use of the `Entity` class.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-541">The following example shows the use of the `Entity` class.</span></span>

```csharp
using System;

class Test
{
    static void Main() {
        Entity.SetNextSerialNo(1000);
        Entity e1 = new Entity();
        Entity e2 = new Entity();
        Console.WriteLine(e1.GetSerialNo());           // Outputs "1000"
        Console.WriteLine(e2.GetSerialNo());           // Outputs "1001"
        Console.WriteLine(Entity.GetNextSerialNo());   // Outputs "1002"
    }
}
```
<span data-ttu-id="7eb1a-542">Note that the `SetNextSerialNo` and `GetNextSerialNo` static methods are invoked on the class whereas the `GetSerialNo` instance method is invoked on instances of the class.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-542">Note that the `SetNextSerialNo` and `GetNextSerialNo` static methods are invoked on the class whereas the `GetSerialNo` instance method is invoked on instances of the class.</span></span>

#### <a name="virtual-override-and-abstract-methods"></a><span data-ttu-id="7eb1a-543">Virtual, override, and abstract methods</span><span class="sxs-lookup"><span data-stu-id="7eb1a-543">Virtual, override, and abstract methods</span></span>

<span data-ttu-id="7eb1a-544">When an instance method declaration includes a `virtual` modifier, the method is said to be a ***virtual method***.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-544">When an instance method declaration includes a `virtual` modifier, the method is said to be a ***virtual method***.</span></span> <span data-ttu-id="7eb1a-545">When no `virtual` modifier is present, the method is said to be a ***non-virtual method***.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-545">When no `virtual` modifier is present, the method is said to be a ***non-virtual method***.</span></span>

<span data-ttu-id="7eb1a-546">When a virtual method is invoked, the ***run-time type*** of the instance for which that invocation takes place determines the actual method implementation to invoke.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-546">When a virtual method is invoked, the ***run-time type*** of the instance for which that invocation takes place determines the actual method implementation to invoke.</span></span> <span data-ttu-id="7eb1a-547">In a nonvirtual method invocation, the ***compile-time type*** of the instance is the determining factor.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-547">In a nonvirtual method invocation, the ***compile-time type*** of the instance is the determining factor.</span></span>

<span data-ttu-id="7eb1a-548">A virtual method can be ***overridden*** in a derived class.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-548">A virtual method can be ***overridden*** in a derived class.</span></span> <span data-ttu-id="7eb1a-549">When an instance method declaration includes an `override` modifier, the method overrides an inherited virtual method with the same signature.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-549">When an instance method declaration includes an `override` modifier, the method overrides an inherited virtual method with the same signature.</span></span> <span data-ttu-id="7eb1a-550">Whereas a virtual method declaration introduces a new method, an override method declaration specializes an existing inherited virtual method by providing a new implementation of that method.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-550">Whereas a virtual method declaration introduces a new method, an override method declaration specializes an existing inherited virtual method by providing a new implementation of that method.</span></span>

<span data-ttu-id="7eb1a-551">An ***abstract*** method is a virtual method with no implementation.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-551">An ***abstract*** method is a virtual method with no implementation.</span></span> <span data-ttu-id="7eb1a-552">An abstract method is declared with the `abstract` modifier and is permitted only in a class that is also declared `abstract`.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-552">An abstract method is declared with the `abstract` modifier and is permitted only in a class that is also declared `abstract`.</span></span> <span data-ttu-id="7eb1a-553">An abstract method must be overridden in every non-abstract derived class.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-553">An abstract method must be overridden in every non-abstract derived class.</span></span>

<span data-ttu-id="7eb1a-554">The following example declares an abstract class, `Expression`, which represents an expression tree node, and three derived classes, `Constant`, `VariableReference`, and `Operation`, which implement expression tree nodes for constants, variable references, and arithmetic operations.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-554">The following example declares an abstract class, `Expression`, which represents an expression tree node, and three derived classes, `Constant`, `VariableReference`, and `Operation`, which implement expression tree nodes for constants, variable references, and arithmetic operations.</span></span> <span data-ttu-id="7eb1a-555">(This is similar to, but not to be confused with the expression tree types introduced in [Expression tree types](types.md#expression-tree-types)).</span><span class="sxs-lookup"><span data-stu-id="7eb1a-555">(This is similar to, but not to be confused with the expression tree types introduced in [Expression tree types](types.md#expression-tree-types)).</span></span>

```csharp
using System;
using System.Collections;

public abstract class Expression
{
    public abstract double Evaluate(Hashtable vars);
}

public class Constant: Expression
{
    double value;

    public Constant(double value) {
        this.value = value;
    }

    public override double Evaluate(Hashtable vars) {
        return value;
    }
}

public class VariableReference: Expression
{
    string name;

    public VariableReference(string name) {
        this.name = name;
    }

    public override double Evaluate(Hashtable vars) {
        object value = vars[name];
        if (value == null) {
            throw new Exception("Unknown variable: " + name);
        }
        return Convert.ToDouble(value);
    }
}

public class Operation: Expression
{
    Expression left;
    char op;
    Expression right;

    public Operation(Expression left, char op, Expression right) {
        this.left = left;
        this.op = op;
        this.right = right;
    }

    public override double Evaluate(Hashtable vars) {
        double x = left.Evaluate(vars);
        double y = right.Evaluate(vars);
        switch (op) {
            case '+': return x + y;
            case '-': return x - y;
            case '*': return x * y;
            case '/': return x / y;
        }
        throw new Exception("Unknown operator");
    }
}
```
<span data-ttu-id="7eb1a-556">The previous four classes can be used to model arithmetic expressions.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-556">The previous four classes can be used to model arithmetic expressions.</span></span> <span data-ttu-id="7eb1a-557">For example, using instances of these classes, the expression `x + 3` can be represented as follows.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-557">For example, using instances of these classes, the expression `x + 3` can be represented as follows.</span></span>

```csharp
Expression e = new Operation(
    new VariableReference("x"),
    '+',
    new Constant(3));
```
<span data-ttu-id="7eb1a-558">The `Evaluate` method of an `Expression` instance is invoked to evaluate the given expression and produce a `double` value.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-558">The `Evaluate` method of an `Expression` instance is invoked to evaluate the given expression and produce a `double` value.</span></span> <span data-ttu-id="7eb1a-559">The method takes as an argument a `Hashtable` that contains variable names (as keys of the entries) and values (as values of the entries).</span><span class="sxs-lookup"><span data-stu-id="7eb1a-559">The method takes as an argument a `Hashtable` that contains variable names (as keys of the entries) and values (as values of the entries).</span></span> <span data-ttu-id="7eb1a-560">The `Evaluate` method is a virtual abstract method, meaning that non-abstract derived classes must override it to provide an actual implementation.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-560">The `Evaluate` method is a virtual abstract method, meaning that non-abstract derived classes must override it to provide an actual implementation.</span></span>

<span data-ttu-id="7eb1a-561">A `Constant`'s implementation of `Evaluate` simply returns the stored constant.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-561">A `Constant`'s implementation of `Evaluate` simply returns the stored constant.</span></span> <span data-ttu-id="7eb1a-562">A `VariableReference`'s implementation looks up the variable name in the hashtable and returns the resulting value.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-562">A `VariableReference`'s implementation looks up the variable name in the hashtable and returns the resulting value.</span></span> <span data-ttu-id="7eb1a-563">An `Operation`'s implementation first evaluates the left and right operands (by recursively invoking their `Evaluate` methods) and then performs the given arithmetic operation.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-563">An `Operation`'s implementation first evaluates the left and right operands (by recursively invoking their `Evaluate` methods) and then performs the given arithmetic operation.</span></span>

<span data-ttu-id="7eb1a-564">The following program uses the `Expression` classes to evaluate the expression `x * (y + 2)` for different values of `x` and `y`.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-564">The following program uses the `Expression` classes to evaluate the expression `x * (y + 2)` for different values of `x` and `y`.</span></span>

```csharp
using System;
using System.Collections;

class Test
{
    static void Main() {
        Expression e = new Operation(
            new VariableReference("x"),
            '*',
            new Operation(
                new VariableReference("y"),
                '+',
                new Constant(2)
            )
        );
        Hashtable vars = new Hashtable();
        vars["x"] = 3;
        vars["y"] = 5;
        Console.WriteLine(e.Evaluate(vars));        // Outputs "21"
        vars["x"] = 1.5;
        vars["y"] = 9;
        Console.WriteLine(e.Evaluate(vars));        // Outputs "16.5"
    }
}
```

#### <a name="method-overloading"></a><span data-ttu-id="7eb1a-565">Method overloading</span><span class="sxs-lookup"><span data-stu-id="7eb1a-565">Method overloading</span></span>

<span data-ttu-id="7eb1a-566">Method ***overloading*** permits multiple methods in the same class to have the same name as long as they have unique signatures.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-566">Method ***overloading*** permits multiple methods in the same class to have the same name as long as they have unique signatures.</span></span> <span data-ttu-id="7eb1a-567">When compiling an invocation of an overloaded method, the compiler uses ***overload resolution*** to determine the specific method to invoke.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-567">When compiling an invocation of an overloaded method, the compiler uses ***overload resolution*** to determine the specific method to invoke.</span></span> <span data-ttu-id="7eb1a-568">Overload resolution finds the one method that best matches the arguments or reports an error if no single best match can be found.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-568">Overload resolution finds the one method that best matches the arguments or reports an error if no single best match can be found.</span></span> <span data-ttu-id="7eb1a-569">The following example shows overload resolution in effect.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-569">The following example shows overload resolution in effect.</span></span> <span data-ttu-id="7eb1a-570">The comment for each invocation in the `Main` method shows which method is actually invoked.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-570">The comment for each invocation in the `Main` method shows which method is actually invoked.</span></span>

```csharp
class Test
{
    static void F() {
        Console.WriteLine("F()");
    }

    static void F(object x) {
        Console.WriteLine("F(object)");
    }

    static void F(int x) {
        Console.WriteLine("F(int)");
    }

    static void F(double x) {
        Console.WriteLine("F(double)");
    }

    static void F<T>(T x) {
        Console.WriteLine("F<T>(T)");
    }

    static void F(double x, double y) {
        Console.WriteLine("F(double, double)");
    }

    static void Main() {
        F();                 // Invokes F()
        F(1);                // Invokes F(int)
        F(1.0);              // Invokes F(double)
        F("abc");            // Invokes F(object)
        F((double)1);        // Invokes F(double)
        F((object)1);        // Invokes F(object)
        F<int>(1);           // Invokes F<T>(T)
        F(1, 1);             // Invokes F(double, double)
    }
}
```
<span data-ttu-id="7eb1a-571">As shown by the example, a particular method can always be selected by explicitly casting the arguments to the exact parameter types and/or explicitly supplying type arguments.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-571">As shown by the example, a particular method can always be selected by explicitly casting the arguments to the exact parameter types and/or explicitly supplying type arguments.</span></span>

### <a name="other-function-members"></a><span data-ttu-id="7eb1a-572">Other function members</span><span class="sxs-lookup"><span data-stu-id="7eb1a-572">Other function members</span></span>

<span data-ttu-id="7eb1a-573">Members that contain executable code are collectively known as the ***function members*** of a class.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-573">Members that contain executable code are collectively known as the ***function members*** of a class.</span></span> <span data-ttu-id="7eb1a-574">The preceding section describes methods, which are the primary kind of function members.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-574">The preceding section describes methods, which are the primary kind of function members.</span></span> <span data-ttu-id="7eb1a-575">This section describes the other kinds of function members supported by C#: constructors, properties, indexers, events, operators, and destructors.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-575">This section describes the other kinds of function members supported by C#: constructors, properties, indexers, events, operators, and destructors.</span></span>

<span data-ttu-id="7eb1a-576">The following code shows a generic class called `List<T>`, which implements a growable list of objects.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-576">The following code shows a generic class called `List<T>`, which implements a growable list of objects.</span></span> <span data-ttu-id="7eb1a-577">The class contains several examples of the most common kinds of function members.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-577">The class contains several examples of the most common kinds of function members.</span></span>


```csharp
public class List<T> {
    // Constant...
    const int defaultCapacity = 4;

    // Fields...
    T[] items;
    int count;

    // Constructors...
    public List(int capacity = defaultCapacity) {
        items = new T[capacity];
    }

    // Properties...
    public int Count {
        get { return count; }
    }
    public int Capacity {
        get {
            return items.Length;
        }
        set {
            if (value < count) value = count;
            if (value != items.Length) {
                T[] newItems = new T[value];
                Array.Copy(items, 0, newItems, 0, count);
                items = newItems;
            }
        }
    }

    // Indexer...
    public T this[int index] {
        get {
            return items[index];
        }
        set {
            items[index] = value;
            OnChanged();
        }
    }

    // Methods...
    public void Add(T item) {
        if (count == Capacity) Capacity = count * 2;
        items[count] = item;
        count++;
        OnChanged();
    }
    protected virtual void OnChanged() {
        if (Changed != null) Changed(this, EventArgs.Empty);
    }
    public override bool Equals(object other) {
        return Equals(this, other as List<T>);
    }
    static bool Equals(List<T> a, List<T> b) {
        if (a == null) return b == null;
        if (b == null || a.count != b.count) return false;
        for (int i = 0; i < a.count; i++) {
            if (!object.Equals(a.items[i], b.items[i])) {
                return false;
            }
        }
        return true;
    }

    // Event...
    public event EventHandler Changed;

    // Operators...
    public static bool operator ==(List<T> a, List<T> b) {
        return Equals(a, b);
    }
    public static bool operator !=(List<T> a, List<T> b) {
        return !Equals(a, b);
    }
}
```

#### <a name="constructors"></a><span data-ttu-id="7eb1a-578">Constructors</span><span class="sxs-lookup"><span data-stu-id="7eb1a-578">Constructors</span></span>

<span data-ttu-id="7eb1a-579">C# supports both instance and static constructors.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-579">C# supports both instance and static constructors.</span></span> <span data-ttu-id="7eb1a-580">An ***instance constructor*** is a member that implements the actions required to initialize an instance of a class.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-580">An ***instance constructor*** is a member that implements the actions required to initialize an instance of a class.</span></span> <span data-ttu-id="7eb1a-581">A ***static constructor*** is a member that implements the actions required to initialize a class itself when it is first loaded.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-581">A ***static constructor*** is a member that implements the actions required to initialize a class itself when it is first loaded.</span></span>

<span data-ttu-id="7eb1a-582">A constructor is declared like a method with no return type and the same name as the containing class.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-582">A constructor is declared like a method with no return type and the same name as the containing class.</span></span> <span data-ttu-id="7eb1a-583">If a constructor declaration includes a `static` modifier, it declares a static constructor.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-583">If a constructor declaration includes a `static` modifier, it declares a static constructor.</span></span> <span data-ttu-id="7eb1a-584">Otherwise, it declares an instance constructor.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-584">Otherwise, it declares an instance constructor.</span></span>

<span data-ttu-id="7eb1a-585">Instance constructors can be overloaded.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-585">Instance constructors can be overloaded.</span></span> <span data-ttu-id="7eb1a-586">For example, the `List<T>
` class declares two instance constructors, one with no parameters and one that takes an `int` parameter.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-586">For example, the `List<T>
` class declares two instance constructors, one with no parameters and one that takes an `int` parameter.</span></span> <span data-ttu-id="7eb1a-587">Instance constructors are invoked using the `new` operator.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-587">Instance constructors are invoked using the `new` operator.</span></span> <span data-ttu-id="7eb1a-588">The following statements allocate two `List<string>
` instances using each of the constructors of the `List` class.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-588">The following statements allocate two `List<string>
` instances using each of the constructors of the `List` class.</span></span>

```csharp
List<string> list1 = new List<string>();
List<string> list2 = new List<string>(10);
```
<span data-ttu-id="7eb1a-589">Unlike other members, instance constructors are not inherited, and a class has no instance constructors other than those actually declared in the class.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-589">Unlike other members, instance constructors are not inherited, and a class has no instance constructors other than those actually declared in the class.</span></span> <span data-ttu-id="7eb1a-590">If no instance constructor is supplied for a class, then an empty one with no parameters is automatically provided.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-590">If no instance constructor is supplied for a class, then an empty one with no parameters is automatically provided.</span></span>

#### <a name="properties"></a><span data-ttu-id="7eb1a-591">Properties</span><span class="sxs-lookup"><span data-stu-id="7eb1a-591">Properties</span></span>

<span data-ttu-id="7eb1a-592">***Properties*** are a natural extension of fields.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-592">***Properties*** are a natural extension of fields.</span></span> <span data-ttu-id="7eb1a-593">Both are named members with associated types, and the syntax for accessing fields and properties is the same.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-593">Both are named members with associated types, and the syntax for accessing fields and properties is the same.</span></span> <span data-ttu-id="7eb1a-594">However, unlike fields, properties do not denote storage locations.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-594">However, unlike fields, properties do not denote storage locations.</span></span> <span data-ttu-id="7eb1a-595">Instead, properties have ***accessors*** that specify the statements to be executed when their values are read or written.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-595">Instead, properties have ***accessors*** that specify the statements to be executed when their values are read or written.</span></span>

<span data-ttu-id="7eb1a-596">A property is declared like a field, except that the declaration ends with a `get` accessor and/or a `set` accessor written between the delimiters `{` and `}` instead of ending in a semicolon.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-596">A property is declared like a field, except that the declaration ends with a `get` accessor and/or a `set` accessor written between the delimiters `{` and `}` instead of ending in a semicolon.</span></span> <span data-ttu-id="7eb1a-597">A property that has both a `get` accessor and a `set` accessor is a ***read-write property***, a property that has only a `get` accessor is a ***read-only property***, and a property that has only a `set` accessor is a ***write-only property***.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-597">A property that has both a `get` accessor and a `set` accessor is a ***read-write property***, a property that has only a `get` accessor is a ***read-only property***, and a property that has only a `set` accessor is a ***write-only property***.</span></span>

<span data-ttu-id="7eb1a-598">A `get` accessor corresponds to a parameterless method with a return value of the property type.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-598">A `get` accessor corresponds to a parameterless method with a return value of the property type.</span></span> <span data-ttu-id="7eb1a-599">Except as the target of an assignment, when a property is referenced in an expression, the `get` accessor of the property is invoked to compute the value of the property.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-599">Except as the target of an assignment, when a property is referenced in an expression, the `get` accessor of the property is invoked to compute the value of the property.</span></span>

<span data-ttu-id="7eb1a-600">A `set` accessor corresponds to a method with a single parameter named `value` and no return type.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-600">A `set` accessor corresponds to a method with a single parameter named `value` and no return type.</span></span> <span data-ttu-id="7eb1a-601">When a property is referenced as the target of an assignment or as the operand of `++` or `--`, the `set` accessor is invoked with an argument that provides the new value.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-601">When a property is referenced as the target of an assignment or as the operand of `++` or `--`, the `set` accessor is invoked with an argument that provides the new value.</span></span>

<span data-ttu-id="7eb1a-602">The `List<T>
` class declares two properties, `Count` and `Capacity`, which are read-only and read-write, respectively.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-602">The `List<T>
` class declares two properties, `Count` and `Capacity`, which are read-only and read-write, respectively.</span></span> <span data-ttu-id="7eb1a-603">The following is an example of use of these properties.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-603">The following is an example of use of these properties.</span></span>

```csharp
List<string> names = new List<string>();
names.Capacity = 100;            // Invokes set accessor
int i = names.Count;             // Invokes get accessor
int j = names.Capacity;          // Invokes get accessor
```
<span data-ttu-id="7eb1a-604">Similar to fields and methods, C# supports both instance properties and static properties.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-604">Similar to fields and methods, C# supports both instance properties and static properties.</span></span> <span data-ttu-id="7eb1a-605">Static properties are declared with the `static` modifier, and instance properties are declared without it.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-605">Static properties are declared with the `static` modifier, and instance properties are declared without it.</span></span>

<span data-ttu-id="7eb1a-606">The accessor(s) of a property can be virtual.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-606">The accessor(s) of a property can be virtual.</span></span> <span data-ttu-id="7eb1a-607">When a property declaration includes a `virtual`, `abstract`, or `override` modifier, it applies to the accessor(s) of the property.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-607">When a property declaration includes a `virtual`, `abstract`, or `override` modifier, it applies to the accessor(s) of the property.</span></span>

#### <a name="indexers"></a><span data-ttu-id="7eb1a-608">Indexers</span><span class="sxs-lookup"><span data-stu-id="7eb1a-608">Indexers</span></span>

<span data-ttu-id="7eb1a-609">An ***indexer*** is a member that enables objects to be indexed in the same way as an array.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-609">An ***indexer*** is a member that enables objects to be indexed in the same way as an array.</span></span> <span data-ttu-id="7eb1a-610">An indexer is declared like a property except that the name of the member is `this` followed by a parameter list written between the delimiters `[` and `]`.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-610">An indexer is declared like a property except that the name of the member is `this` followed by a parameter list written between the delimiters `[` and `]`.</span></span> <span data-ttu-id="7eb1a-611">The parameters are available in the accessor(s) of the indexer.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-611">The parameters are available in the accessor(s) of the indexer.</span></span> <span data-ttu-id="7eb1a-612">Similar to properties, indexers can be read-write, read-only, and write-only, and the accessor(s) of an indexer can be virtual.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-612">Similar to properties, indexers can be read-write, read-only, and write-only, and the accessor(s) of an indexer can be virtual.</span></span>

<span data-ttu-id="7eb1a-613">The `List` class declares a single read-write indexer that takes an `int` parameter.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-613">The `List` class declares a single read-write indexer that takes an `int` parameter.</span></span> <span data-ttu-id="7eb1a-614">The indexer makes it possible to index `List` instances with `int` values.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-614">The indexer makes it possible to index `List` instances with `int` values.</span></span> <span data-ttu-id="7eb1a-615">For example</span><span class="sxs-lookup"><span data-stu-id="7eb1a-615">For example</span></span>

```csharp
List<string> names = new List<string>();
names.Add("Liz");
names.Add("Martha");
names.Add("Beth");
for (int i = 0; i < names.Count; i++) {
    string s = names[i];
    names[i] = s.ToUpper();
}
```
<span data-ttu-id="7eb1a-616">Indexers can be overloaded, meaning that a class can declare multiple indexers as long as the number or types of their parameters differ.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-616">Indexers can be overloaded, meaning that a class can declare multiple indexers as long as the number or types of their parameters differ.</span></span>

#### <a name="events"></a><span data-ttu-id="7eb1a-617">Events</span><span class="sxs-lookup"><span data-stu-id="7eb1a-617">Events</span></span>

<span data-ttu-id="7eb1a-618">An ***event*** is a member that enables a class or object to provide notifications.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-618">An ***event*** is a member that enables a class or object to provide notifications.</span></span> <span data-ttu-id="7eb1a-619">An event is declared like a field except that the declaration includes an `event` keyword and the type must be a delegate type.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-619">An event is declared like a field except that the declaration includes an `event` keyword and the type must be a delegate type.</span></span>

<span data-ttu-id="7eb1a-620">Within a class that declares an event member, the event behaves just like a field of a delegate type (provided the event is not abstract and does not declare accessors).</span><span class="sxs-lookup"><span data-stu-id="7eb1a-620">Within a class that declares an event member, the event behaves just like a field of a delegate type (provided the event is not abstract and does not declare accessors).</span></span> <span data-ttu-id="7eb1a-621">The field stores a reference to a delegate that represents the event handlers that have been added to the event.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-621">The field stores a reference to a delegate that represents the event handlers that have been added to the event.</span></span> <span data-ttu-id="7eb1a-622">If no event handles are present, the field is `null`.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-622">If no event handles are present, the field is `null`.</span></span>

<span data-ttu-id="7eb1a-623">The `List<T>
` class declares a single event member called `Changed`, which indicates that a new item has been added to the list.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-623">The `List<T>
` class declares a single event member called `Changed`, which indicates that a new item has been added to the list.</span></span> <span data-ttu-id="7eb1a-624">The `Changed` event is raised by the `OnChanged` virtual method, which first checks whether the event is `null` (meaning that no handlers are present).</span><span class="sxs-lookup"><span data-stu-id="7eb1a-624">The `Changed` event is raised by the `OnChanged` virtual method, which first checks whether the event is `null` (meaning that no handlers are present).</span></span> <span data-ttu-id="7eb1a-625">The notion of raising an event is precisely equivalent to invoking the delegate represented by the event—thus, there are no special language constructs for raising events.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-625">The notion of raising an event is precisely equivalent to invoking the delegate represented by the event—thus, there are no special language constructs for raising events.</span></span>

<span data-ttu-id="7eb1a-626">Clients react to events through ***event handlers***.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-626">Clients react to events through ***event handlers***.</span></span> <span data-ttu-id="7eb1a-627">Event handlers are attached using the `+=` operator and removed using the `-=` operator.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-627">Event handlers are attached using the `+=` operator and removed using the `-=` operator.</span></span> <span data-ttu-id="7eb1a-628">The following example attaches an event handler to the `Changed` event of a `List<string>
`.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-628">The following example attaches an event handler to the `Changed` event of a `List<string>
`.</span></span>

```csharp
using System;

class Test
{
    static int changeCount;

    static void ListChanged(object sender, EventArgs e) {
        changeCount++;
    }

    static void Main() {
        List<string> names = new List<string>();
        names.Changed += new EventHandler(ListChanged);
        names.Add("Liz");
        names.Add("Martha");
        names.Add("Beth");
        Console.WriteLine(changeCount);        // Outputs "3"
    }
}
```
<span data-ttu-id="7eb1a-629">For advanced scenarios where control of the underlying storage of an event is desired, an event declaration can explicitly provide `add` and `remove` accessors, which are somewhat similar to the `set` accessor of a property.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-629">For advanced scenarios where control of the underlying storage of an event is desired, an event declaration can explicitly provide `add` and `remove` accessors, which are somewhat similar to the `set` accessor of a property.</span></span>

#### <a name="operators"></a><span data-ttu-id="7eb1a-630">Operators</span><span class="sxs-lookup"><span data-stu-id="7eb1a-630">Operators</span></span>

<span data-ttu-id="7eb1a-631">An ***operator*** is a member that defines the meaning of applying a particular expression operator to instances of a class.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-631">An ***operator*** is a member that defines the meaning of applying a particular expression operator to instances of a class.</span></span> <span data-ttu-id="7eb1a-632">Three kinds of operators can be defined: unary operators, binary operators, and conversion operators.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-632">Three kinds of operators can be defined: unary operators, binary operators, and conversion operators.</span></span> <span data-ttu-id="7eb1a-633">All operators must be declared as `public` and `static`.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-633">All operators must be declared as `public` and `static`.</span></span>

<span data-ttu-id="7eb1a-634">The `List<T>
` class declares two operators, `operator==` and `operator!=`, and thus gives new meaning to expressions that apply those operators to `List` instances.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-634">The `List<T>
` class declares two operators, `operator==` and `operator!=`, and thus gives new meaning to expressions that apply those operators to `List` instances.</span></span> <span data-ttu-id="7eb1a-635">Specifically, the operators define equality of two `List<T>
` instances as comparing each of the contained objects using their `Equals` methods.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-635">Specifically, the operators define equality of two `List<T>
` instances as comparing each of the contained objects using their `Equals` methods.</span></span> <span data-ttu-id="7eb1a-636">The following example uses the `==` operator to compare two `List<int>
` instances.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-636">The following example uses the `==` operator to compare two `List<int>
` instances.</span></span>

```csharp
using System;

class Test
{
    static void Main() {
        List<int> a = new List<int>();
        a.Add(1);
        a.Add(2);
        List<int> b = new List<int>();
        b.Add(1);
        b.Add(2);
        Console.WriteLine(a == b);        // Outputs "True"
        b.Add(3);
        Console.WriteLine(a == b);        // Outputs "False"
    }
}
```

<span data-ttu-id="7eb1a-637">The first `Console.WriteLine` outputs `True` because the two lists contain the same number of objects with the same values in the same order.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-637">The first `Console.WriteLine` outputs `True` because the two lists contain the same number of objects with the same values in the same order.</span></span> <span data-ttu-id="7eb1a-638">Had `List<T>
` not defined `operator==`, the first `Console.WriteLine` would have output `False` because `a` and `b` reference different `List<int>
` instances.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-638">Had `List<T>
` not defined `operator==`, the first `Console.WriteLine` would have output `False` because `a` and `b` reference different `List<int>
` instances.</span></span>

#### <a name="destructors"></a><span data-ttu-id="7eb1a-639">Destructors</span><span class="sxs-lookup"><span data-stu-id="7eb1a-639">Destructors</span></span>

<span data-ttu-id="7eb1a-640">A ***destructor*** is a member that implements the actions required to destruct an instance of a class.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-640">A ***destructor*** is a member that implements the actions required to destruct an instance of a class.</span></span> <span data-ttu-id="7eb1a-641">Destructors cannot have parameters, they cannot have accessibility modifiers, and they cannot be invoked explicitly.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-641">Destructors cannot have parameters, they cannot have accessibility modifiers, and they cannot be invoked explicitly.</span></span> <span data-ttu-id="7eb1a-642">The destructor for an instance is invoked automatically during garbage collection.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-642">The destructor for an instance is invoked automatically during garbage collection.</span></span>

<span data-ttu-id="7eb1a-643">The garbage collector is allowed wide latitude in deciding when to collect objects and run destructors.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-643">The garbage collector is allowed wide latitude in deciding when to collect objects and run destructors.</span></span> <span data-ttu-id="7eb1a-644">Specifically, the timing of destructor invocations is not deterministic, and destructors may be executed on any thread.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-644">Specifically, the timing of destructor invocations is not deterministic, and destructors may be executed on any thread.</span></span> <span data-ttu-id="7eb1a-645">For these and other reasons, classes should implement destructors only when no other solutions are feasible.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-645">For these and other reasons, classes should implement destructors only when no other solutions are feasible.</span></span>

<span data-ttu-id="7eb1a-646">The `using` statement provides a better approach to object destruction.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-646">The `using` statement provides a better approach to object destruction.</span></span>

## <a name="structs"></a><span data-ttu-id="7eb1a-647">Structs</span><span class="sxs-lookup"><span data-stu-id="7eb1a-647">Structs</span></span>

<span data-ttu-id="7eb1a-648">Like classes, ***structs*** are data structures that can contain data members and function members, but unlike classes, structs are value types and do not require heap allocation.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-648">Like classes, ***structs*** are data structures that can contain data members and function members, but unlike classes, structs are value types and do not require heap allocation.</span></span> <span data-ttu-id="7eb1a-649">A variable of a struct type directly stores the data of the struct, whereas a variable of a class type stores a reference to a dynamically allocated object.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-649">A variable of a struct type directly stores the data of the struct, whereas a variable of a class type stores a reference to a dynamically allocated object.</span></span> <span data-ttu-id="7eb1a-650">Struct types do not support user-specified inheritance, and all struct types implicitly inherit from type `object`.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-650">Struct types do not support user-specified inheritance, and all struct types implicitly inherit from type `object`.</span></span>

<span data-ttu-id="7eb1a-651">Structs are particularly useful for small data structures that have value semantics.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-651">Structs are particularly useful for small data structures that have value semantics.</span></span> <span data-ttu-id="7eb1a-652">Complex numbers, points in a coordinate system, or key-value pairs in a dictionary are all good examples of structs.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-652">Complex numbers, points in a coordinate system, or key-value pairs in a dictionary are all good examples of structs.</span></span> <span data-ttu-id="7eb1a-653">The use of structs rather than classes for small data structures can make a large difference in the number of memory allocations an application performs.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-653">The use of structs rather than classes for small data structures can make a large difference in the number of memory allocations an application performs.</span></span> <span data-ttu-id="7eb1a-654">For example, the following program creates and initializes an array of 100 points.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-654">For example, the following program creates and initializes an array of 100 points.</span></span> <span data-ttu-id="7eb1a-655">With `Point` implemented as a class, 101 separate objects are instantiated—one for the array and one each for the 100 elements.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-655">With `Point` implemented as a class, 101 separate objects are instantiated—one for the array and one each for the 100 elements.</span></span>

```csharp
class Point
{
    public int x, y;

    public Point(int x, int y) {
        this.x = x;
        this.y = y;
    }
}

class Test
{
    static void Main() {
        Point[] points = new Point[100];
        for (int i = 0; i < 100; i++) points[i] = new Point(i, i);
    }
}
```
<span data-ttu-id="7eb1a-656">An alternative is to make `Point` a struct.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-656">An alternative is to make `Point` a struct.</span></span>

```csharp
struct Point
{
    public int x, y;

    public Point(int x, int y) {
        this.x = x;
        this.y = y;
    }
}
```
<span data-ttu-id="7eb1a-657">Now, only one object is instantiated—the one for the array—and the `Point` instances are stored in-line in the array.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-657">Now, only one object is instantiated—the one for the array—and the `Point` instances are stored in-line in the array.</span></span>

<span data-ttu-id="7eb1a-658">Struct constructors are invoked with the `new` operator, but that does not imply that memory is being allocated.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-658">Struct constructors are invoked with the `new` operator, but that does not imply that memory is being allocated.</span></span> <span data-ttu-id="7eb1a-659">Instead of dynamically allocating an object and returning a reference to it, a struct constructor simply returns the struct value itself (typically in a temporary location on the stack), and this value is then copied as necessary.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-659">Instead of dynamically allocating an object and returning a reference to it, a struct constructor simply returns the struct value itself (typically in a temporary location on the stack), and this value is then copied as necessary.</span></span>

<span data-ttu-id="7eb1a-660">With classes, it is possible for two variables to reference the same object and thus possible for operations on one variable to affect the object referenced by the other variable.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-660">With classes, it is possible for two variables to reference the same object and thus possible for operations on one variable to affect the object referenced by the other variable.</span></span> <span data-ttu-id="7eb1a-661">With structs, the variables each have their own copy of the data, and it is not possible for operations on one to affect the other.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-661">With structs, the variables each have their own copy of the data, and it is not possible for operations on one to affect the other.</span></span> <span data-ttu-id="7eb1a-662">For example, the output produced by the following code fragment depends on whether `Point` is a class or a struct.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-662">For example, the output produced by the following code fragment depends on whether `Point` is a class or a struct.</span></span>

```csharp
Point a = new Point(10, 10);
Point b = a;
a.x = 20;
Console.WriteLine(b.x);
```
<span data-ttu-id="7eb1a-663">If `Point` is a class, the output is `20` because `a` and `b` reference the same object.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-663">If `Point` is a class, the output is `20` because `a` and `b` reference the same object.</span></span> <span data-ttu-id="7eb1a-664">If `Point` is a struct, the output is `10` because the assignment of `a` to `b` creates a copy of the value, and this copy is unaffected by the subsequent assignment to `a.x`.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-664">If `Point` is a struct, the output is `10` because the assignment of `a` to `b` creates a copy of the value, and this copy is unaffected by the subsequent assignment to `a.x`.</span></span>

<span data-ttu-id="7eb1a-665">The previous example highlights two of the limitations of structs.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-665">The previous example highlights two of the limitations of structs.</span></span> <span data-ttu-id="7eb1a-666">First, copying an entire struct is typically less efficient than copying an object reference, so assignment and value parameter passing can be more expensive with structs than with reference types.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-666">First, copying an entire struct is typically less efficient than copying an object reference, so assignment and value parameter passing can be more expensive with structs than with reference types.</span></span> <span data-ttu-id="7eb1a-667">Second, except for `ref` and `out` parameters, it is not possible to create references to structs, which rules out their usage in a number of situations.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-667">Second, except for `ref` and `out` parameters, it is not possible to create references to structs, which rules out their usage in a number of situations.</span></span>

## <a name="arrays"></a><span data-ttu-id="7eb1a-668">Arrays</span><span class="sxs-lookup"><span data-stu-id="7eb1a-668">Arrays</span></span>

<span data-ttu-id="7eb1a-669">An ***array*** is a data structure that contains a number of variables that are accessed through computed indices.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-669">An ***array*** is a data structure that contains a number of variables that are accessed through computed indices.</span></span> <span data-ttu-id="7eb1a-670">The variables contained in an array, also called the ***elements*** of the array, are all of the same type, and this type is called the ***element type*** of the array.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-670">The variables contained in an array, also called the ***elements*** of the array, are all of the same type, and this type is called the ***element type*** of the array.</span></span>

<span data-ttu-id="7eb1a-671">Array types are reference types, and the declaration of an array variable simply sets aside space for a reference to an array instance.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-671">Array types are reference types, and the declaration of an array variable simply sets aside space for a reference to an array instance.</span></span> <span data-ttu-id="7eb1a-672">Actual array instances are created dynamically at run-time using the `new` operator.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-672">Actual array instances are created dynamically at run-time using the `new` operator.</span></span> <span data-ttu-id="7eb1a-673">The `new` operation specifies the ***length*** of the new array instance, which is then fixed for the lifetime of the instance.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-673">The `new` operation specifies the ***length*** of the new array instance, which is then fixed for the lifetime of the instance.</span></span> <span data-ttu-id="7eb1a-674">The indices of the elements of an array range from `0` to `Length - 1`.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-674">The indices of the elements of an array range from `0` to `Length - 1`.</span></span> <span data-ttu-id="7eb1a-675">The `new` operator automatically initializes the elements of an array to their default value, which, for example, is zero for all numeric types and `null` for all reference types.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-675">The `new` operator automatically initializes the elements of an array to their default value, which, for example, is zero for all numeric types and `null` for all reference types.</span></span>

<span data-ttu-id="7eb1a-676">The following example creates an array of `int` elements, initializes the array, and prints out the contents of the array.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-676">The following example creates an array of `int` elements, initializes the array, and prints out the contents of the array.</span></span>

```csharp
using System;

class Test
{
    static void Main() {
        int[] a = new int[10];
        for (int i = 0; i < a.Length; i++) {
            a[i] = i * i;
        }
        for (int i = 0; i < a.Length; i++) {
            Console.WriteLine("a[{0}] = {1}", i, a[i]);
        }
    }
}
```
<span data-ttu-id="7eb1a-677">This example creates and operates on a ***single-dimensional array***.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-677">This example creates and operates on a ***single-dimensional array***.</span></span> <span data-ttu-id="7eb1a-678">C# also supports ***multi-dimensional arrays***.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-678">C# also supports ***multi-dimensional arrays***.</span></span> <span data-ttu-id="7eb1a-679">The number of dimensions of an array type, also known as the ***rank*** of the array type, is one plus the number of commas written between the square brackets of the array type.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-679">The number of dimensions of an array type, also known as the ***rank*** of the array type, is one plus the number of commas written between the square brackets of the array type.</span></span> <span data-ttu-id="7eb1a-680">The following example allocates a one-dimensional, a two-dimensional, and a three-dimensional array.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-680">The following example allocates a one-dimensional, a two-dimensional, and a three-dimensional array.</span></span>

```csharp
int[] a1 = new int[10];
int[,] a2 = new int[10, 5];
int[,,] a3 = new int[10, 5, 2];
```
<span data-ttu-id="7eb1a-681">The `a1` array contains 10 elements, the `a2` array contains 50 (10 × 5) elements, and the `a3` array contains 100 (10 × 5 × 2) elements.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-681">The `a1` array contains 10 elements, the `a2` array contains 50 (10 × 5) elements, and the `a3` array contains 100 (10 × 5 × 2) elements.</span></span>

<span data-ttu-id="7eb1a-682">The element type of an array can be any type, including an array type.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-682">The element type of an array can be any type, including an array type.</span></span> <span data-ttu-id="7eb1a-683">An array with elements of an array type is sometimes called a ***jagged array*** because the lengths of the element arrays do not all have to be the same.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-683">An array with elements of an array type is sometimes called a ***jagged array*** because the lengths of the element arrays do not all have to be the same.</span></span> <span data-ttu-id="7eb1a-684">The following example allocates an array of arrays of `int`:</span><span class="sxs-lookup"><span data-stu-id="7eb1a-684">The following example allocates an array of arrays of `int`:</span></span>

```csharp
int[][] a = new int[3][];
a[0] = new int[10];
a[1] = new int[5];
a[2] = new int[20];
```
<span data-ttu-id="7eb1a-685">The first line creates an array with three elements, each of type `int[]` and each with an initial value of `null`.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-685">The first line creates an array with three elements, each of type `int[]` and each with an initial value of `null`.</span></span> <span data-ttu-id="7eb1a-686">The subsequent lines then initialize the three elements with references to individual array instances of varying lengths.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-686">The subsequent lines then initialize the three elements with references to individual array instances of varying lengths.</span></span>

<span data-ttu-id="7eb1a-687">The `new` operator permits the initial values of the array elements to be specified using an ***array initializer***, which is a list of expressions written between the delimiters `{` and `}`.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-687">The `new` operator permits the initial values of the array elements to be specified using an ***array initializer***, which is a list of expressions written between the delimiters `{` and `}`.</span></span> <span data-ttu-id="7eb1a-688">The following example allocates and initializes an `int[]` with three elements.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-688">The following example allocates and initializes an `int[]` with three elements.</span></span>

```csharp
int[] a = new int[] {1, 2, 3};
```
<span data-ttu-id="7eb1a-689">Note that the length of the array is inferred from the number of expressions between `{` and `}`.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-689">Note that the length of the array is inferred from the number of expressions between `{` and `}`.</span></span> <span data-ttu-id="7eb1a-690">Local variable and field declarations can be shortened further such that the array type does not have to be restated.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-690">Local variable and field declarations can be shortened further such that the array type does not have to be restated.</span></span>

```csharp
int[] a = {1, 2, 3};
```
<span data-ttu-id="7eb1a-691">Both of the previous examples are equivalent to the following:</span><span class="sxs-lookup"><span data-stu-id="7eb1a-691">Both of the previous examples are equivalent to the following:</span></span>

```csharp
int[] t = new int[3];
t[0] = 1;
t[1] = 2;
t[2] = 3;
int[] a = t;
```
## <a name="interfaces"></a><span data-ttu-id="7eb1a-692">Interfaces</span><span class="sxs-lookup"><span data-stu-id="7eb1a-692">Interfaces</span></span>

<span data-ttu-id="7eb1a-693">An ***interface*** defines a contract that can be implemented by classes and structs.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-693">An ***interface*** defines a contract that can be implemented by classes and structs.</span></span> <span data-ttu-id="7eb1a-694">An interface can contain methods, properties, events, and indexers.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-694">An interface can contain methods, properties, events, and indexers.</span></span> <span data-ttu-id="7eb1a-695">An interface does not provide implementations of the members it defines—it merely specifies the members that must be supplied by classes or structs that implement the interface.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-695">An interface does not provide implementations of the members it defines—it merely specifies the members that must be supplied by classes or structs that implement the interface.</span></span>

<span data-ttu-id="7eb1a-696">Interfaces may employ ***multiple inheritance***.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-696">Interfaces may employ ***multiple inheritance***.</span></span> <span data-ttu-id="7eb1a-697">In the following example, the interface `IComboBox` inherits from both `ITextBox` and `IListBox`.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-697">In the following example, the interface `IComboBox` inherits from both `ITextBox` and `IListBox`.</span></span>

```csharp
interface IControl
{
    void Paint();
}

interface ITextBox: IControl
{
    void SetText(string text);
}

interface IListBox: IControl
{
    void SetItems(string[] items);
}

interface IComboBox: ITextBox, IListBox {}
```
<span data-ttu-id="7eb1a-698">Classes and structs can implement multiple interfaces.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-698">Classes and structs can implement multiple interfaces.</span></span> <span data-ttu-id="7eb1a-699">In the following example, the class `EditBox` implements both `IControl` and `IDataBound`.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-699">In the following example, the class `EditBox` implements both `IControl` and `IDataBound`.</span></span>

```csharp
interface IDataBound
{
    void Bind(Binder b);
}

public class EditBox: IControl, IDataBound
{
    public void Paint() {...}
    public void Bind(Binder b) {...}
}
```
<span data-ttu-id="7eb1a-700">When a class or struct implements a particular interface, instances of that class or struct can be implicitly converted to that interface type.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-700">When a class or struct implements a particular interface, instances of that class or struct can be implicitly converted to that interface type.</span></span> <span data-ttu-id="7eb1a-701">For example</span><span class="sxs-lookup"><span data-stu-id="7eb1a-701">For example</span></span>

```csharp
EditBox editBox = new EditBox();
IControl control = editBox;
IDataBound dataBound = editBox;
```
<span data-ttu-id="7eb1a-702">In cases where an instance is not statically known to implement a particular interface, dynamic type casts can be used.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-702">In cases where an instance is not statically known to implement a particular interface, dynamic type casts can be used.</span></span> <span data-ttu-id="7eb1a-703">For example, the following statements use dynamic type casts to obtain an object's `IControl` and `IDataBound` interface implementations.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-703">For example, the following statements use dynamic type casts to obtain an object's `IControl` and `IDataBound` interface implementations.</span></span> <span data-ttu-id="7eb1a-704">Because the actual type of the object is `EditBox`, the casts succeed.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-704">Because the actual type of the object is `EditBox`, the casts succeed.</span></span>

```csharp
object obj = new EditBox();
IControl control = (IControl)obj;
IDataBound dataBound = (IDataBound)obj;
```
<span data-ttu-id="7eb1a-705">In the previous `EditBox` class, the `Paint` method from the `IControl` interface and the `Bind` method from the `IDataBound` interface are implemented using `public` members.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-705">In the previous `EditBox` class, the `Paint` method from the `IControl` interface and the `Bind` method from the `IDataBound` interface are implemented using `public` members.</span></span> <span data-ttu-id="7eb1a-706">C# also supports ***explicit interface member implementations***, using which the class or struct can avoid making the members `public`.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-706">C# also supports ***explicit interface member implementations***, using which the class or struct can avoid making the members `public`.</span></span> <span data-ttu-id="7eb1a-707">An explicit interface member implementation is written using the fully qualified interface member name.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-707">An explicit interface member implementation is written using the fully qualified interface member name.</span></span> <span data-ttu-id="7eb1a-708">For example, the `EditBox` class could implement the `IControl.Paint` and `IDataBound.Bind` methods using explicit interface member implementations as follows.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-708">For example, the `EditBox` class could implement the `IControl.Paint` and `IDataBound.Bind` methods using explicit interface member implementations as follows.</span></span>

```csharp
public class EditBox: IControl, IDataBound
{
    void IControl.Paint() {...}
    void IDataBound.Bind(Binder b) {...}
}
```
<span data-ttu-id="7eb1a-709">Explicit interface members can only be accessed via the interface type.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-709">Explicit interface members can only be accessed via the interface type.</span></span> <span data-ttu-id="7eb1a-710">For example, the implementation of `IControl.Paint` provided by the previous `EditBox` class can only be invoked by first converting the `EditBox` reference to the `IControl` interface type.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-710">For example, the implementation of `IControl.Paint` provided by the previous `EditBox` class can only be invoked by first converting the `EditBox` reference to the `IControl` interface type.</span></span>

```csharp
EditBox editBox = new EditBox();
editBox.Paint();                        // Error, no such method
IControl control = editBox;
control.Paint();                        // Ok
```

## <a name="enums"></a><span data-ttu-id="7eb1a-711">Enums</span><span class="sxs-lookup"><span data-stu-id="7eb1a-711">Enums</span></span>

<span data-ttu-id="7eb1a-712">An ***enum type*** is a distinct value type with a set of named constants.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-712">An ***enum type*** is a distinct value type with a set of named constants.</span></span> <span data-ttu-id="7eb1a-713">The following example declares and uses an enum type named `Color` with three constant values, `Red`, `Green`, and `Blue`.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-713">The following example declares and uses an enum type named `Color` with three constant values, `Red`, `Green`, and `Blue`.</span></span>

```csharp
using System;

enum Color
{
    Red,
    Green,
    Blue
}

class Test
{
    static void PrintColor(Color color) {
        switch (color) {
            case Color.Red:
                Console.WriteLine("Red");
                break;
            case Color.Green:
                Console.WriteLine("Green");
                break;
            case Color.Blue:
                Console.WriteLine("Blue");
                break;
            default:
                Console.WriteLine("Unknown color");
                break;
        }
    }

    static void Main() {
        Color c = Color.Red;
        PrintColor(c);
        PrintColor(Color.Blue);
    }
}
```
<span data-ttu-id="7eb1a-714">Each enum type has a corresponding integral type called the ***underlying type*** of the enum type.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-714">Each enum type has a corresponding integral type called the ***underlying type*** of the enum type.</span></span> <span data-ttu-id="7eb1a-715">An enum type that does not explicitly declare an underlying type has an underlying type of `int`.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-715">An enum type that does not explicitly declare an underlying type has an underlying type of `int`.</span></span> <span data-ttu-id="7eb1a-716">An enum type's storage format and range of possible values are determined by its underlying type.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-716">An enum type's storage format and range of possible values are determined by its underlying type.</span></span> <span data-ttu-id="7eb1a-717">The set of values that an enum type can take on is not limited by its enum members.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-717">The set of values that an enum type can take on is not limited by its enum members.</span></span> <span data-ttu-id="7eb1a-718">In particular, any value of the underlying type of an enum can be cast to the enum type and is a distinct valid value of that enum type.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-718">In particular, any value of the underlying type of an enum can be cast to the enum type and is a distinct valid value of that enum type.</span></span>

<span data-ttu-id="7eb1a-719">The following example declares an enum type named `Alignment` with an underlying type of `sbyte`.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-719">The following example declares an enum type named `Alignment` with an underlying type of `sbyte`.</span></span>

```csharp
enum Alignment: sbyte
{
    Left = -1,
    Center = 0,
    Right = 1
}
```
<span data-ttu-id="7eb1a-720">As shown by the previous example, an enum member declaration can include a constant expression that specifies the value of the member.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-720">As shown by the previous example, an enum member declaration can include a constant expression that specifies the value of the member.</span></span> <span data-ttu-id="7eb1a-721">The constant value for each enum member must be in the range of the underlying type of the enum.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-721">The constant value for each enum member must be in the range of the underlying type of the enum.</span></span> <span data-ttu-id="7eb1a-722">When an enum member declaration does not explicitly specify a value, the member is given the value zero (if it is the first member in the enum type) or the value of the textually preceding enum member plus one.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-722">When an enum member declaration does not explicitly specify a value, the member is given the value zero (if it is the first member in the enum type) or the value of the textually preceding enum member plus one.</span></span>

<span data-ttu-id="7eb1a-723">Enum values can be converted to integral values and vice versa using type casts.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-723">Enum values can be converted to integral values and vice versa using type casts.</span></span> <span data-ttu-id="7eb1a-724">For example</span><span class="sxs-lookup"><span data-stu-id="7eb1a-724">For example</span></span>

```csharp
int i = (int)Color.Blue;        // int i = 2;
Color c = (Color)2;             // Color c = Color.Blue;
```
<span data-ttu-id="7eb1a-725">The default value of any enum type is the integral value zero converted to the enum type.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-725">The default value of any enum type is the integral value zero converted to the enum type.</span></span> <span data-ttu-id="7eb1a-726">In cases where variables are automatically initialized to a default value, this is the value given to variables of enum types.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-726">In cases where variables are automatically initialized to a default value, this is the value given to variables of enum types.</span></span> <span data-ttu-id="7eb1a-727">In order for the default value of an enum type to be easily available, the literal `0` implicitly converts to any enum type.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-727">In order for the default value of an enum type to be easily available, the literal `0` implicitly converts to any enum type.</span></span> <span data-ttu-id="7eb1a-728">Thus, the following is permitted.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-728">Thus, the following is permitted.</span></span>

```csharp
Color c = 0;
```

## <a name="delegates"></a><span data-ttu-id="7eb1a-729">Delegates</span><span class="sxs-lookup"><span data-stu-id="7eb1a-729">Delegates</span></span>

<span data-ttu-id="7eb1a-730">A ***delegate type*** represents references to methods with a particular parameter list and return type.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-730">A ***delegate type*** represents references to methods with a particular parameter list and return type.</span></span> <span data-ttu-id="7eb1a-731">Delegates make it possible to treat methods as entities that can be assigned to variables and passed as parameters.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-731">Delegates make it possible to treat methods as entities that can be assigned to variables and passed as parameters.</span></span> <span data-ttu-id="7eb1a-732">Delegates are similar to the concept of function pointers found in some other languages, but unlike function pointers, delegates are object-oriented and type-safe.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-732">Delegates are similar to the concept of function pointers found in some other languages, but unlike function pointers, delegates are object-oriented and type-safe.</span></span>

<span data-ttu-id="7eb1a-733">The following example declares and uses a delegate type named `Function`.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-733">The following example declares and uses a delegate type named `Function`.</span></span>

```csharp
using System;

delegate double Function(double x);

class Multiplier
{
    double factor;

    public Multiplier(double factor) {
        this.factor = factor;
    }

    public double Multiply(double x) {
        return x * factor;
    }
}

class Test
{
    static double Square(double x) {
        return x * x;
    }

    static double[] Apply(double[] a, Function f) {
        double[] result = new double[a.Length];
        for (int i = 0; i < a.Length; i++) result[i] = f(a[i]);
        return result;
    }

    static void Main() {
        double[] a = {0.0, 0.5, 1.0};
        double[] squares = Apply(a, Square);
        double[] sines = Apply(a, Math.Sin);
        Multiplier m = new Multiplier(2.0);
        double[] doubles =  Apply(a, m.Multiply);
    }
}
```
<span data-ttu-id="7eb1a-734">An instance of the `Function` delegate type can reference any method that takes a `double` argument and returns a `double` value.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-734">An instance of the `Function` delegate type can reference any method that takes a `double` argument and returns a `double` value.</span></span> <span data-ttu-id="7eb1a-735">The `Apply` method applies a given `Function` to the elements of a `double[]`, returning a `double[]` with the results.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-735">The `Apply` method applies a given `Function` to the elements of a `double[]`, returning a `double[]` with the results.</span></span> <span data-ttu-id="7eb1a-736">In the `Main` method, `Apply` is used to apply three different functions to a `double[]`.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-736">In the `Main` method, `Apply` is used to apply three different functions to a `double[]`.</span></span>

<span data-ttu-id="7eb1a-737">A delegate can reference either a static method (such as `Square` or `Math.Sin` in the previous example) or an instance method (such as `m.Multiply` in the previous example).</span><span class="sxs-lookup"><span data-stu-id="7eb1a-737">A delegate can reference either a static method (such as `Square` or `Math.Sin` in the previous example) or an instance method (such as `m.Multiply` in the previous example).</span></span> <span data-ttu-id="7eb1a-738">A delegate that references an instance method also references a particular object, and when the instance method is invoked through the delegate, that object becomes `this` in the invocation.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-738">A delegate that references an instance method also references a particular object, and when the instance method is invoked through the delegate, that object becomes `this` in the invocation.</span></span>

<span data-ttu-id="7eb1a-739">Delegates can also be created using anonymous functions, which are "inline methods" that are created on the fly.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-739">Delegates can also be created using anonymous functions, which are "inline methods" that are created on the fly.</span></span> <span data-ttu-id="7eb1a-740">Anonymous functions can see the local variables of the surrounding methods.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-740">Anonymous functions can see the local variables of the surrounding methods.</span></span> <span data-ttu-id="7eb1a-741">Thus, the multiplier example above can be written more easily without using a `Multiplier` class:</span><span class="sxs-lookup"><span data-stu-id="7eb1a-741">Thus, the multiplier example above can be written more easily without using a `Multiplier` class:</span></span>

```csharp
double[] doubles =  Apply(a, (double x) => x * 2.0);
```
<span data-ttu-id="7eb1a-742">An interesting and useful property of a delegate is that it does not know or care about the class of the method it references; all that matters is that the referenced method has the same parameters and return type as the delegate.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-742">An interesting and useful property of a delegate is that it does not know or care about the class of the method it references; all that matters is that the referenced method has the same parameters and return type as the delegate.</span></span>

## <a name="attributes"></a><span data-ttu-id="7eb1a-743">Attributes</span><span class="sxs-lookup"><span data-stu-id="7eb1a-743">Attributes</span></span>

<span data-ttu-id="7eb1a-744">Types, members, and other entities in a C# program support modifiers that control certain aspects of their behavior.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-744">Types, members, and other entities in a C# program support modifiers that control certain aspects of their behavior.</span></span> <span data-ttu-id="7eb1a-745">For example, the accessibility of a method is controlled using the `public`, `protected`, `internal`, and `private` modifiers.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-745">For example, the accessibility of a method is controlled using the `public`, `protected`, `internal`, and `private` modifiers.</span></span> <span data-ttu-id="7eb1a-746">C# generalizes this capability such that user-defined types of declarative information can be attached to program entities and retrieved at run-time.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-746">C# generalizes this capability such that user-defined types of declarative information can be attached to program entities and retrieved at run-time.</span></span> <span data-ttu-id="7eb1a-747">Programs specify this additional declarative information by defining and using ***attributes***.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-747">Programs specify this additional declarative information by defining and using ***attributes***.</span></span>

<span data-ttu-id="7eb1a-748">The following example declares a `HelpAttribute` attribute that can be placed on program entities to provide links to their associated documentation.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-748">The following example declares a `HelpAttribute` attribute that can be placed on program entities to provide links to their associated documentation.</span></span>

```csharp
using System;

public class HelpAttribute: Attribute
{
    string url;
    string topic;

    public HelpAttribute(string url) {
        this.url = url;
    }

    public string Url {
        get { return url; }
    }

    public string Topic {
        get { return topic; }
        set { topic = value; }
    }
}
```
<span data-ttu-id="7eb1a-749">All attribute classes derive from the `System.Attribute` base class provided by the .NET Framework.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-749">All attribute classes derive from the `System.Attribute` base class provided by the .NET Framework.</span></span> <span data-ttu-id="7eb1a-750">Attributes can be applied by giving their name, along with any arguments, inside square brackets just before the associated declaration.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-750">Attributes can be applied by giving their name, along with any arguments, inside square brackets just before the associated declaration.</span></span> <span data-ttu-id="7eb1a-751">If an attribute's name ends in `Attribute`, that part of the name can be omitted when the attribute is referenced.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-751">If an attribute's name ends in `Attribute`, that part of the name can be omitted when the attribute is referenced.</span></span> <span data-ttu-id="7eb1a-752">For example, the `HelpAttribute` attribute can be used as follows.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-752">For example, the `HelpAttribute` attribute can be used as follows.</span></span>

```csharp
[Help("http://msdn.microsoft.com/.../MyClass.htm")]
public class Widget
{
    [Help("http://msdn.microsoft.com/.../MyClass.htm", Topic = "Display")]
    public void Display(string text) {}
}
```
<span data-ttu-id="7eb1a-753">This example attaches a `HelpAttribute` to the `Widget` class and another `HelpAttribute` to the `Display` method in the class.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-753">This example attaches a `HelpAttribute` to the `Widget` class and another `HelpAttribute` to the `Display` method in the class.</span></span> <span data-ttu-id="7eb1a-754">The public constructors of an attribute class control the information that must be provided when the attribute is attached to a program entity.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-754">The public constructors of an attribute class control the information that must be provided when the attribute is attached to a program entity.</span></span> <span data-ttu-id="7eb1a-755">Additional information can be provided by referencing public read-write properties of the attribute class (such as the reference to the `Topic` property previously).</span><span class="sxs-lookup"><span data-stu-id="7eb1a-755">Additional information can be provided by referencing public read-write properties of the attribute class (such as the reference to the `Topic` property previously).</span></span>

<span data-ttu-id="7eb1a-756">The following example shows how attribute information for a given program entity can be retrieved at run-time using reflection.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-756">The following example shows how attribute information for a given program entity can be retrieved at run-time using reflection.</span></span>

```csharp
using System;
using System.Reflection;

class Test
{
    static void ShowHelp(MemberInfo member) {
        HelpAttribute a = Attribute.GetCustomAttribute(member,
            typeof(HelpAttribute)) as HelpAttribute;
        if (a == null) {
            Console.WriteLine("No help for {0}", member);
        }
        else {
            Console.WriteLine("Help for {0}:", member);
            Console.WriteLine("  Url={0}, Topic={1}", a.Url, a.Topic);
        }
    }

    static void Main() {
        ShowHelp(typeof(Widget));
        ShowHelp(typeof(Widget).GetMethod("Display"));
    }
}
```
<span data-ttu-id="7eb1a-757">When a particular attribute is requested through reflection, the constructor for the attribute class is invoked with the information provided in the program source, and the resulting attribute instance is returned.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-757">When a particular attribute is requested through reflection, the constructor for the attribute class is invoked with the information provided in the program source, and the resulting attribute instance is returned.</span></span> <span data-ttu-id="7eb1a-758">If additional information was provided through properties, those properties are set to the given values before the attribute instance is returned.This is test</span><span class="sxs-lookup"><span data-stu-id="7eb1a-758">If additional information was provided through properties, those properties are set to the given values before the attribute instance is returned.This is test</span></span>
