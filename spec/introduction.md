# <a name="introduction"></a><span data-ttu-id="73d35-101">介绍</span><span class="sxs-lookup"><span data-stu-id="73d35-101">Introduction</span></span>

<span data-ttu-id="73d35-102">C#（读作“See Sharp”）是一种简单易用的新式编程语言，不仅面向对象，还类型安全。</span><span class="sxs-lookup"><span data-stu-id="73d35-102">C# (pronounced "See Sharp") is a simple, modern, object-oriented, and type-safe programming language.</span></span> <span data-ttu-id="73d35-103">C# 起源于 C 语言系列，将立即为 C、 c + + 和 Java 编程人员所熟悉。</span><span class="sxs-lookup"><span data-stu-id="73d35-103">C# has its roots in the C family of languages and will be immediately familiar to C, C++, and Java programmers.</span></span> <span data-ttu-id="73d35-104">C# 的标准化为 ECMA international ***ECMA-334***标准和通过为 ISO/IEC ***ISO/IEC 23270***标准。</span><span class="sxs-lookup"><span data-stu-id="73d35-104">C# is standardized by ECMA International as the ***ECMA-334*** standard and by ISO/IEC as the ***ISO/IEC 23270*** standard.</span></span> <span data-ttu-id="73d35-105">Microsoft 的 C# 编译器为.NET Framework 是一致的这两个这些标准实现。</span><span class="sxs-lookup"><span data-stu-id="73d35-105">Microsoft's C# compiler for the .NET Framework is a conforming implementation of both of these standards.</span></span>

<span data-ttu-id="73d35-106">C# 是一种面向对象的语言。不仅如此，C# 还进一步支持***面向组件的***编程。</span><span class="sxs-lookup"><span data-stu-id="73d35-106">C# is an object-oriented language, but C# further includes support for ***component-oriented*** programming.</span></span> <span data-ttu-id="73d35-107">当代软件设计越来越依赖采用自描述的独立功能包形式的软件组件。</span><span class="sxs-lookup"><span data-stu-id="73d35-107">Contemporary software design increasingly relies on software components in the form of self-contained and self-describing packages of functionality.</span></span> <span data-ttu-id="73d35-108">此类组件的关键特征包括：为编程模型提供属性、方法和事件；包含提供组件声明性信息的特性；包含自己的文档。</span><span class="sxs-lookup"><span data-stu-id="73d35-108">Key to such components is that they present a programming model with properties, methods, and events; they have attributes that provide declarative information about the component; and they incorporate their own documentation.</span></span> <span data-ttu-id="73d35-109">C# 提供语言构造来直接支持这些概念，使 C# 中用于创建和使用软件组件非常自然的语言。</span><span class="sxs-lookup"><span data-stu-id="73d35-109">C# provides language constructs to directly support these concepts, making C# a very natural language in which to create and use software components.</span></span>

<span data-ttu-id="73d35-110">多个C#功能的可靠且持久应用程序构造中的帮助：***垃圾回收***自动回收未使用的对象; 占用的内存***异常处理***提供了错误检测和恢复; 的结构化和可扩展方法并***类型安全***语言的设计使它无法读取未初始化的变量，索引超出其边界或执行未选中状态的数组类型强制转换。</span><span class="sxs-lookup"><span data-stu-id="73d35-110">Several C# features aid in the construction of robust and durable applications: ***Garbage collection*** automatically reclaims memory occupied by unused objects; ***exception handling*** provides a structured and extensible approach to error detection and recovery; and the ***type-safe*** design of the language makes it impossible to read from uninitialized variables, to index arrays beyond their bounds, or to perform unchecked type casts.</span></span>

<span data-ttu-id="73d35-111">C# 采用***统一的类型系统***。</span><span class="sxs-lookup"><span data-stu-id="73d35-111">C# has a ***unified type system***.</span></span> <span data-ttu-id="73d35-112">所有 C# 类型（包括 `int` 和 `double` 等基元类型）均继承自一个根 `object` 类型。</span><span class="sxs-lookup"><span data-stu-id="73d35-112">All C# types, including primitive types such as `int` and `double`, inherit from a single root `object` type.</span></span> <span data-ttu-id="73d35-113">因此，所有类型共用一组通用运算，任何类型的值都可以一致地进行存储、传输和处理。</span><span class="sxs-lookup"><span data-stu-id="73d35-113">Thus, all types share a set of common operations, and values of any type can be stored, transported, and operated upon in a consistent manner.</span></span> <span data-ttu-id="73d35-114">此外，C# 还支持用户定义的引用类型和值类型，从而支持对象动态分配以及轻量级结构的内嵌式存储。</span><span class="sxs-lookup"><span data-stu-id="73d35-114">Furthermore, C# supports both user-defined reference types and value types, allowing dynamic allocation of objects as well as in-line storage of lightweight structures.</span></span>

<span data-ttu-id="73d35-115">若要确保，C# 程序和库可以改进随着时间的推移以兼容的方式，更强调上***版本控制***在 C# 的设计。</span><span class="sxs-lookup"><span data-stu-id="73d35-115">To ensure that C# programs and libraries can evolve over time in a compatible manner, much emphasis has been placed on ***versioning*** in C#'s design.</span></span> <span data-ttu-id="73d35-116">许多编程语言很少关注这个问题，因此，当引入新版依赖库时，用这些语言编写的程序会出现更多不必要的中断现象。</span><span class="sxs-lookup"><span data-stu-id="73d35-116">Many programming languages pay little attention to this issue, and, as a result, programs written in those languages break more often than necessary when newer versions of dependent libraries are introduced.</span></span> <span data-ttu-id="73d35-117">直接受版本控制考虑事项的 C# 设计方面包括单独`virtual`和`override`修饰符、 关于方法重载决策规则和显式接口成员声明的支持。</span><span class="sxs-lookup"><span data-stu-id="73d35-117">Aspects of C#'s design that were directly influenced by versioning considerations include the separate `virtual` and `override` modifiers, the rules for method overload resolution, and support for explicit interface member declarations.</span></span>

<span data-ttu-id="73d35-118">本章的其余部分介绍 C# 语言的基本功能。</span><span class="sxs-lookup"><span data-stu-id="73d35-118">The rest of this chapter describes the essential features of the C# language.</span></span> <span data-ttu-id="73d35-119">尽管更高版本的章节介绍了面向详细信息的且有时数学的方式的规则和例外，这一章致力于清晰和简洁起见，但要牺牲完整性的考虑。</span><span class="sxs-lookup"><span data-stu-id="73d35-119">Although later chapters describe rules and exceptions in a detail-oriented and sometimes mathematical manner, this chapter strives for clarity and brevity at the expense of completeness.</span></span> <span data-ttu-id="73d35-120">目的是介绍如何将有助于开始编写程序的写入和读取后面的章节的语言提供读取器。</span><span class="sxs-lookup"><span data-stu-id="73d35-120">The intent is to provide the reader with an introduction to the language that will facilitate the writing of early programs and the reading of later chapters.</span></span>

## <a name="hello-world"></a><span data-ttu-id="73d35-121">Hello world</span><span class="sxs-lookup"><span data-stu-id="73d35-121">Hello world</span></span>

<span data-ttu-id="73d35-122">“Hello, World”程序历来都用于介绍编程语言。</span><span class="sxs-lookup"><span data-stu-id="73d35-122">The "Hello, World" program is traditionally used to introduce a programming language.</span></span> <span data-ttu-id="73d35-123">下面展示了此程序的 C# 代码：</span><span class="sxs-lookup"><span data-stu-id="73d35-123">Here it is in C#:</span></span>

```csharp
using System;

class Hello
{
    static void Main() {
        Console.WriteLine("Hello, World");
    }
}
```

<span data-ttu-id="73d35-124">C# 源文件的文件扩展名通常为 `.cs`。</span><span class="sxs-lookup"><span data-stu-id="73d35-124">C# source files typically have the file extension `.cs`.</span></span> <span data-ttu-id="73d35-125">假设"Hello，World"程序存储在文件`hello.cs`，可以使用 Microsoft C# 编译器使用命令行编译该程序</span><span class="sxs-lookup"><span data-stu-id="73d35-125">Assuming that the "Hello, World" program is stored in the file `hello.cs`, the program can be compiled with the Microsoft C# compiler using the command line</span></span>
```
csc hello.cs
```
<span data-ttu-id="73d35-126">这会生成名为可执行程序集`hello.exe`。</span><span class="sxs-lookup"><span data-stu-id="73d35-126">which produces an executable assembly named `hello.exe`.</span></span> <span data-ttu-id="73d35-127">此应用程序运行时生成的输出是</span><span class="sxs-lookup"><span data-stu-id="73d35-127">The output produced by this application when it is run is</span></span>
```
Hello, World
```

<span data-ttu-id="73d35-128">“Hello, World”程序始于引用 `System` 命名空间的 `using` 指令。</span><span class="sxs-lookup"><span data-stu-id="73d35-128">The "Hello, World" program starts with a `using` directive that references the `System` namespace.</span></span> <span data-ttu-id="73d35-129">命名空间提供了一种用于组织 C# 程序和库的分层方法。</span><span class="sxs-lookup"><span data-stu-id="73d35-129">Namespaces provide a hierarchical means of organizing C# programs and libraries.</span></span> <span data-ttu-id="73d35-130">命名空间包含类型和其他命名空间。例如，`System` 命名空间包含许多类型（如程序中引用的 `Console` 类）和其他许多命名空间（如 `IO` 和 `Collections`）。</span><span class="sxs-lookup"><span data-stu-id="73d35-130">Namespaces contain types and other namespaces—for example, the `System` namespace contains a number of types, such as the `Console` class referenced in the program, and a number of other namespaces, such as `IO` and `Collections`.</span></span> <span data-ttu-id="73d35-131">借助引用给定命名空间的 `using` 指令，可以非限定的方式使用作为相应命名空间成员的类型。</span><span class="sxs-lookup"><span data-stu-id="73d35-131">A `using` directive that references a given namespace enables unqualified use of the types that are members of that namespace.</span></span> <span data-ttu-id="73d35-132">由于使用 `using` 指令，因此程序可以使用 `Console.WriteLine` 作为 `System.Console.WriteLine` 的简写。</span><span class="sxs-lookup"><span data-stu-id="73d35-132">Because of the `using` directive, the program can use `Console.WriteLine` as shorthand for `System.Console.WriteLine`.</span></span>

<span data-ttu-id="73d35-133">“Hello, World”程序声明的 `Hello` 类只有一个成员，即 `Main` 方法。</span><span class="sxs-lookup"><span data-stu-id="73d35-133">The `Hello` class declared by the "Hello, World" program has a single member, the method named `Main`.</span></span> <span data-ttu-id="73d35-134">`Main`方法声明具有`static`修饰符。</span><span class="sxs-lookup"><span data-stu-id="73d35-134">The `Main` method is declared with the `static` modifier.</span></span> <span data-ttu-id="73d35-135">实例方法可以使用关键字 `this` 引用特定的封闭对象实例，而静态方法则可以在不引用特定对象的情况下运行。</span><span class="sxs-lookup"><span data-stu-id="73d35-135">While instance methods can reference a particular enclosing object instance using the keyword `this`, static methods operate without reference to a particular object.</span></span> <span data-ttu-id="73d35-136">按照约定，`Main` 静态方法是程序的入口点。</span><span class="sxs-lookup"><span data-stu-id="73d35-136">By convention, a static method named `Main` serves as the entry point of a program.</span></span>

<span data-ttu-id="73d35-137">程序的输出是由 `System` 命名空间中 `Console` 类的 `WriteLine` 方法生成。</span><span class="sxs-lookup"><span data-stu-id="73d35-137">The output of the program is produced by the `WriteLine` method of the `Console` class in the `System` namespace.</span></span> <span data-ttu-id="73d35-138">此类提供的.NET Framework 类库，其中，默认情况下，将自动引用由 Microsoft C# 编译器。</span><span class="sxs-lookup"><span data-stu-id="73d35-138">This class is provided by the .NET Framework class libraries, which, by default, are automatically referenced by the Microsoft C# compiler.</span></span> <span data-ttu-id="73d35-139">请注意，C# 语言本身没有单独的运行时库。</span><span class="sxs-lookup"><span data-stu-id="73d35-139">Note that C# itself does not have a separate runtime library.</span></span> <span data-ttu-id="73d35-140">相反，.NET Framework 是运行时库的 C#。</span><span class="sxs-lookup"><span data-stu-id="73d35-140">Instead, the .NET Framework is the runtime library of C#.</span></span>

## <a name="program-structure"></a><span data-ttu-id="73d35-141">程序结构</span><span class="sxs-lookup"><span data-stu-id="73d35-141">Program structure</span></span>

<span data-ttu-id="73d35-142">C# 中的关键组织结构概念包括***程序***、***命名空间***、***类型***、***成员***和***程序集***。</span><span class="sxs-lookup"><span data-stu-id="73d35-142">The key organizational concepts in C# are ***programs***, ***namespaces***, ***types***, ***members***, and ***assemblies***.</span></span> <span data-ttu-id="73d35-143">C# 程序由一个或多个源文件组成。</span><span class="sxs-lookup"><span data-stu-id="73d35-143">C# programs consist of one or more source files.</span></span> <span data-ttu-id="73d35-144">程序声明类型，而类型则包含成员，并被整理到命名空间中。</span><span class="sxs-lookup"><span data-stu-id="73d35-144">Programs declare types, which contain members and can be organized into namespaces.</span></span> <span data-ttu-id="73d35-145">类型示例包括类和接口。</span><span class="sxs-lookup"><span data-stu-id="73d35-145">Classes and interfaces are examples of types.</span></span> <span data-ttu-id="73d35-146">成员示例包括字段、方法、属性和事件。</span><span class="sxs-lookup"><span data-stu-id="73d35-146">Fields, methods, properties, and events are examples of members.</span></span> <span data-ttu-id="73d35-147">编译完的 C# 程序实际上会打包到程序集中。</span><span class="sxs-lookup"><span data-stu-id="73d35-147">When C# programs are compiled, they are physically packaged into assemblies.</span></span> <span data-ttu-id="73d35-148">程序集通常具有文件扩展名`.exe`或`.dll`，取决于它们的实现是否***应用程序***或***库***。</span><span class="sxs-lookup"><span data-stu-id="73d35-148">Assemblies typically have the file extension `.exe` or `.dll`, depending on whether they implement ***applications*** or ***libraries***.</span></span>

<span data-ttu-id="73d35-149">该示例</span><span class="sxs-lookup"><span data-stu-id="73d35-149">The example</span></span>

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
<span data-ttu-id="73d35-150">声明一个名为类`Stack`调用的命名空间中`Acme.Collections`。</span><span class="sxs-lookup"><span data-stu-id="73d35-150">declares a class named `Stack` in a namespace called `Acme.Collections`.</span></span> <span data-ttu-id="73d35-151">此类的完全限定的名称为 `Acme.Collections.Stack`。</span><span class="sxs-lookup"><span data-stu-id="73d35-151">The fully qualified name of this class is `Acme.Collections.Stack`.</span></span> <span data-ttu-id="73d35-152">此类包含多个成员：一个 `top` 字段、两个方法（`Push` 和 `Pop`）和一个 `Entry` 嵌套类。</span><span class="sxs-lookup"><span data-stu-id="73d35-152">The class contains several members: a field named `top`, two methods named `Push` and `Pop`, and a nested class named `Entry`.</span></span> <span data-ttu-id="73d35-153">`Entry` 类还包含三个成员：一个 `next` 字段、一个 `data` 字段和一个构造函数。</span><span class="sxs-lookup"><span data-stu-id="73d35-153">The `Entry` class further contains three members: a field named `next`, a field named `data`, and a constructor.</span></span> <span data-ttu-id="73d35-154">假定示例的源代码存储在 `acme.cs` 文件中，以下命令行</span><span class="sxs-lookup"><span data-stu-id="73d35-154">Assuming that the source code of the example is stored in the file `acme.cs`, the command line</span></span>

```
csc /t:library acme.cs
```
<span data-ttu-id="73d35-155">将示例编译成库（不含 `Main` 入口点的代码），并生成 `acme.dll` 程序集。</span><span class="sxs-lookup"><span data-stu-id="73d35-155">compiles the example as a library (code without a `Main` entry point) and produces an assembly named `acme.dll`.</span></span>

<span data-ttu-id="73d35-156">程序集包含可执行代码中的窗体***中间语言***(IL) 指令和符号化信息的形式***元数据***。</span><span class="sxs-lookup"><span data-stu-id="73d35-156">Assemblies contain executable code in the form of ***Intermediate Language*** (IL) instructions, and symbolic information in the form of ***metadata***.</span></span> <span data-ttu-id="73d35-157">执行前，程序集中的 IL 代码会被 .NET 公共语言运行时的实时 (JIT) 编译器自动转换成处理器专属代码。</span><span class="sxs-lookup"><span data-stu-id="73d35-157">Before it is executed, the IL code in an assembly is automatically converted to processor-specific code by the Just-In-Time (JIT) compiler of .NET Common Language Runtime.</span></span>

<span data-ttu-id="73d35-158">由于程序集是包含代码和元数据的自描述功能单元，因此无需在 C# 中使用 `#include` 指令和头文件。</span><span class="sxs-lookup"><span data-stu-id="73d35-158">Because an assembly is a self-describing unit of functionality containing both code and metadata, there is no need for `#include` directives and header files in C#.</span></span> <span data-ttu-id="73d35-159">只需在编译程序时引用特定的程序集，即可在 C# 程序中使用此程序集中包含的公共类型和成员。</span><span class="sxs-lookup"><span data-stu-id="73d35-159">The public types and members contained in a particular assembly are made available in a C# program simply by referencing that assembly when compiling the program.</span></span> <span data-ttu-id="73d35-160">例如，此程序使用 `acme.dll` 程序集中的 `Acme.Collections.Stack` 类：</span><span class="sxs-lookup"><span data-stu-id="73d35-160">For example, this program uses the `Acme.Collections.Stack` class from the `acme.dll` assembly:</span></span>

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
<span data-ttu-id="73d35-161">如果程序存储在文件`test.cs`，当`test.cs`进行编译`acme.dll`可以使用编译器的引用程序集`/r`选项：</span><span class="sxs-lookup"><span data-stu-id="73d35-161">If the program is stored in the file `test.cs`, when `test.cs` is compiled, the `acme.dll` assembly can be referenced using the compiler's `/r` option:</span></span>

```
csc /r:acme.dll test.cs
```
<span data-ttu-id="73d35-162">这会创建 `test.exe` 可执行程序集，它将在运行时输出以下内容：</span><span class="sxs-lookup"><span data-stu-id="73d35-162">This creates an executable assembly named `test.exe`, which, when run, produces the output:</span></span>

```
100
10
1
```
<span data-ttu-id="73d35-163">使用 C#，可以将程序的源文本存储在多个源文件中。</span><span class="sxs-lookup"><span data-stu-id="73d35-163">C# permits the source text of a program to be stored in several source files.</span></span> <span data-ttu-id="73d35-164">编译多文件 C# 程序时，可以将所有源文件一起处理，并且源文件可以随意相互引用。从概念上讲，就像是所有源文件在处理前被集中到一个大文件中一样。</span><span class="sxs-lookup"><span data-stu-id="73d35-164">When a multi-file C# program is compiled, all of the source files are processed together, and the source files can freely reference each other—conceptually, it is as if all the source files were concatenated into one large file before being processed.</span></span> <span data-ttu-id="73d35-165">在 C# 中，永远都不需要使用前向声明，因为声明顺序无关紧要（除了极少数的例外情况）。</span><span class="sxs-lookup"><span data-stu-id="73d35-165">Forward declarations are never needed in C# because, with very few exceptions, declaration order is insignificant.</span></span> <span data-ttu-id="73d35-166">C# 并不限制源文件只能声明一种公共类型，也不要求源文件的文件名必须与其中声明的类型相匹配。</span><span class="sxs-lookup"><span data-stu-id="73d35-166">C# does not limit a source file to declaring only one public type nor does it require the name of the source file to match a type declared in the source file.</span></span>

## <a name="types-and-variables"></a><span data-ttu-id="73d35-167">类型和变量</span><span class="sxs-lookup"><span data-stu-id="73d35-167">Types and variables</span></span>

<span data-ttu-id="73d35-168">C# 有两种类型：***值类型***和***引用类型***。</span><span class="sxs-lookup"><span data-stu-id="73d35-168">There are two kinds of types in C#: ***value types*** and ***reference types***.</span></span> <span data-ttu-id="73d35-169">值类型的变量直接包含数据，而引用类型的变量则存储对数据（称为“对象”）的引用。</span><span class="sxs-lookup"><span data-stu-id="73d35-169">Variables of value types directly contain their data whereas variables of reference types store references to their data, the latter being known as objects.</span></span> <span data-ttu-id="73d35-170">对于引用类型，两个变量可以引用同一对象；因此，对一个变量执行的运算可能会影响另一个变量引用的对象。</span><span class="sxs-lookup"><span data-stu-id="73d35-170">With reference types, it is possible for two variables to reference the same object and thus possible for operations on one variable to affect the object referenced by the other variable.</span></span> <span data-ttu-id="73d35-171">借助值类型，每个变量都有自己的数据副本；因此，对一个变量执行的运算不会影响另一个变量（`ref` 和 `out` 参数变量除外）。</span><span class="sxs-lookup"><span data-stu-id="73d35-171">With value types, the variables each have their own copy of the data, and it is not possible for operations on one to affect the other (except in the case of `ref` and `out` parameter variables).</span></span>

<span data-ttu-id="73d35-172">C# 值类型又细分***简单类型***，***枚举类型***，***结构类型***，以及***可以为 null 类型***，和 C# 参考类型又细分***类类型***，***接口类型***，***数组类型***，以及***委托类型***。</span><span class="sxs-lookup"><span data-stu-id="73d35-172">C#'s value types are further divided into ***simple types***, ***enum types***, ***struct types***, and ***nullable types***, and C#'s reference types are further divided into ***class types***, ***interface types***, ***array types***, and ***delegate types***.</span></span>

<span data-ttu-id="73d35-173">下表提供了 C# 类型系统的概述。</span><span class="sxs-lookup"><span data-stu-id="73d35-173">The following table provides an overview of C#'s type system.</span></span>

| <span data-ttu-id="73d35-174">__类别__</span><span class="sxs-lookup"><span data-stu-id="73d35-174">__Category__</span></span>    |                 | <span data-ttu-id="73d35-175">__说明__</span><span class="sxs-lookup"><span data-stu-id="73d35-175">__Description__</span></span> |
|-----------------|-----------------|-----------------|
| <span data-ttu-id="73d35-176">值类型</span><span class="sxs-lookup"><span data-stu-id="73d35-176">Value types</span></span>     | <span data-ttu-id="73d35-177">简单类型</span><span class="sxs-lookup"><span data-stu-id="73d35-177">Simple types</span></span>    | <span data-ttu-id="73d35-178">有符号的整型：`sbyte`、`short`、`int`、`long`</span><span class="sxs-lookup"><span data-stu-id="73d35-178">Signed integral: `sbyte`, `short`, `int`, `long`</span></span> |
|                 |                 | <span data-ttu-id="73d35-179">无符号的整型：`byte`、`ushort`、`uint`、`ulong`</span><span class="sxs-lookup"><span data-stu-id="73d35-179">Unsigned integral: `byte`, `ushort`, `uint`, `ulong`</span></span> |
|                 |                 | <span data-ttu-id="73d35-180">Unicode 字符：`char`</span><span class="sxs-lookup"><span data-stu-id="73d35-180">Unicode characters: `char`</span></span> |
|                 |                 | <span data-ttu-id="73d35-181">IEEE 浮点：`float`、`double`</span><span class="sxs-lookup"><span data-stu-id="73d35-181">IEEE floating point: `float`, `double`</span></span> |
|                 |                 | <span data-ttu-id="73d35-182">高精度小数：`decimal`</span><span class="sxs-lookup"><span data-stu-id="73d35-182">High-precision decimal: `decimal`</span></span> |
|                 |                 | <span data-ttu-id="73d35-183">布尔：`bool`</span><span class="sxs-lookup"><span data-stu-id="73d35-183">Boolean: `bool`</span></span> |
|                 | <span data-ttu-id="73d35-184">枚举类型</span><span class="sxs-lookup"><span data-stu-id="73d35-184">Enum types</span></span>      | <span data-ttu-id="73d35-185">格式为 `enum E {...}` 的用户定义类型</span><span class="sxs-lookup"><span data-stu-id="73d35-185">User-defined types of the form `enum E {...}`</span></span> |
|                 | <span data-ttu-id="73d35-186">结构类型</span><span class="sxs-lookup"><span data-stu-id="73d35-186">Struct types</span></span>    | <span data-ttu-id="73d35-187">格式为 `struct S {...}` 的用户定义类型</span><span class="sxs-lookup"><span data-stu-id="73d35-187">User-defined types of the form `struct S {...}`</span></span> |
|                 | <span data-ttu-id="73d35-188">可以为 null 的类型</span><span class="sxs-lookup"><span data-stu-id="73d35-188">Nullable types</span></span>  | <span data-ttu-id="73d35-189">值为 `null` 的其他所有值类型的扩展</span><span class="sxs-lookup"><span data-stu-id="73d35-189">Extensions of all other value types with a `null` value</span></span> |
| <span data-ttu-id="73d35-190">引用类型</span><span class="sxs-lookup"><span data-stu-id="73d35-190">Reference types</span></span> | <span data-ttu-id="73d35-191">类类型</span><span class="sxs-lookup"><span data-stu-id="73d35-191">Class types</span></span>     | <span data-ttu-id="73d35-192">其他所有类型的最终基类：`object`</span><span class="sxs-lookup"><span data-stu-id="73d35-192">Ultimate base class of all other types: `object`</span></span> |
|                 |                 | <span data-ttu-id="73d35-193">Unicode 字符串：`string`</span><span class="sxs-lookup"><span data-stu-id="73d35-193">Unicode strings: `string`</span></span> |
|                 |                 | <span data-ttu-id="73d35-194">格式为 `class C {...}` 的用户定义类型</span><span class="sxs-lookup"><span data-stu-id="73d35-194">User-defined types of the form `class C {...}`</span></span> |
|                 | <span data-ttu-id="73d35-195">接口类型</span><span class="sxs-lookup"><span data-stu-id="73d35-195">Interface types</span></span> | <span data-ttu-id="73d35-196">格式为 `interface I {...}` 的用户定义类型</span><span class="sxs-lookup"><span data-stu-id="73d35-196">User-defined types of the form `interface I {...}`</span></span> |
|                 | <span data-ttu-id="73d35-197">数组类型</span><span class="sxs-lookup"><span data-stu-id="73d35-197">Array types</span></span>     | <span data-ttu-id="73d35-198">一维和多维，例如 `int[]` 和 `int[,]`</span><span class="sxs-lookup"><span data-stu-id="73d35-198">Single- and multi-dimensional, for example, `int[]` and `int[,]`</span></span> |
|                 | <span data-ttu-id="73d35-199">委托类型</span><span class="sxs-lookup"><span data-stu-id="73d35-199">Delegate types</span></span>  | <span data-ttu-id="73d35-200">用户定义类型的窗体例如 `delegate int  D(...)`</span><span class="sxs-lookup"><span data-stu-id="73d35-200">User-defined types of the form e.g. `delegate int  D(...)`</span></span> |

<span data-ttu-id="73d35-201">八个整型类型支持带符号或不带符号格式的 8 位、16 位、32 位和 64 位值。</span><span class="sxs-lookup"><span data-stu-id="73d35-201">The eight integral types provide support for 8-bit, 16-bit, 32-bit, and 64-bit values in signed or unsigned form.</span></span>

<span data-ttu-id="73d35-202">两个浮动点类型，`float`和`double`，使用 32 位单精度和 64 位双精度 IEEE 754 格式表示。</span><span class="sxs-lookup"><span data-stu-id="73d35-202">The two floating point types, `float` and `double`, are represented using the 32-bit single-precision and 64-bit double-precision IEEE 754 formats.</span></span>

<span data-ttu-id="73d35-203">`decimal` 类型是适用于财务和货币计算的 128 位数据类型。</span><span class="sxs-lookup"><span data-stu-id="73d35-203">The `decimal` type is a 128-bit data type suitable for financial and monetary calculations.</span></span>

<span data-ttu-id="73d35-204">C#`bool`类型用于表示布尔值 — 值要么`true`或`false`。</span><span class="sxs-lookup"><span data-stu-id="73d35-204">C#'s `bool` type is used to represent boolean values—values that are either `true` or `false`.</span></span>

<span data-ttu-id="73d35-205">C# 使用 Unicode 编码处理字符和字符串。</span><span class="sxs-lookup"><span data-stu-id="73d35-205">Character and string processing in C# uses Unicode encoding.</span></span> <span data-ttu-id="73d35-206">`char` 类型表示 UTF-16 代码单元，`string` 类型表示一系列 UTF-16 代码单元。</span><span class="sxs-lookup"><span data-stu-id="73d35-206">The `char` type represents a UTF-16 code unit, and the `string` type represents a sequence of UTF-16 code units.</span></span>

<span data-ttu-id="73d35-207">下表总结了 C# 的数值类型。</span><span class="sxs-lookup"><span data-stu-id="73d35-207">The following table summarizes C#'s numeric types.</span></span>


| <span data-ttu-id="73d35-208">__类别__</span><span class="sxs-lookup"><span data-stu-id="73d35-208">__Category__</span></span>      | <span data-ttu-id="73d35-209">__Bits__</span><span class="sxs-lookup"><span data-stu-id="73d35-209">__Bits__</span></span> | <span data-ttu-id="73d35-210">__Type__</span><span class="sxs-lookup"><span data-stu-id="73d35-210">__Type__</span></span>  | <span data-ttu-id="73d35-211">__作用域/精度__</span><span class="sxs-lookup"><span data-stu-id="73d35-211">__Range/Precision__</span></span> |
|-------------------|----------|-----------|---------------------|
| <span data-ttu-id="73d35-212">有符号的整型</span><span class="sxs-lookup"><span data-stu-id="73d35-212">Signed integral</span></span>   | <span data-ttu-id="73d35-213">8</span><span class="sxs-lookup"><span data-stu-id="73d35-213">8</span></span>        | `sbyte`   | <span data-ttu-id="73d35-214">-128...127</span><span class="sxs-lookup"><span data-stu-id="73d35-214">-128...127</span></span> |
|                   | <span data-ttu-id="73d35-215">16</span><span class="sxs-lookup"><span data-stu-id="73d35-215">16</span></span>       | `short`   | <span data-ttu-id="73d35-216">-32,768...32,767</span><span class="sxs-lookup"><span data-stu-id="73d35-216">-32,768...32,767</span></span> |
|                   | <span data-ttu-id="73d35-217">32</span><span class="sxs-lookup"><span data-stu-id="73d35-217">32</span></span>       | `int`     | <span data-ttu-id="73d35-218">-2,147,483,648...2,147,483,647</span><span class="sxs-lookup"><span data-stu-id="73d35-218">-2,147,483,648...2,147,483,647</span></span> |
|                   | <span data-ttu-id="73d35-219">64</span><span class="sxs-lookup"><span data-stu-id="73d35-219">64</span></span>       | `long`    | <span data-ttu-id="73d35-220">-9,223,372,036,854,775,808...9,223,372,036,854,775,807</span><span class="sxs-lookup"><span data-stu-id="73d35-220">-9,223,372,036,854,775,808...9,223,372,036,854,775,807</span></span> |
| <span data-ttu-id="73d35-221">无符号的整型</span><span class="sxs-lookup"><span data-stu-id="73d35-221">Unsigned integral</span></span> | <span data-ttu-id="73d35-222">8</span><span class="sxs-lookup"><span data-stu-id="73d35-222">8</span></span>        | `byte`    | <span data-ttu-id="73d35-223">0...255</span><span class="sxs-lookup"><span data-stu-id="73d35-223">0...255</span></span> |
|                   | <span data-ttu-id="73d35-224">16</span><span class="sxs-lookup"><span data-stu-id="73d35-224">16</span></span>       | `ushort`  | <span data-ttu-id="73d35-225">0...65,535</span><span class="sxs-lookup"><span data-stu-id="73d35-225">0...65,535</span></span> |
|                   | <span data-ttu-id="73d35-226">32</span><span class="sxs-lookup"><span data-stu-id="73d35-226">32</span></span>       | `uint`    | <span data-ttu-id="73d35-227">0...4,294,967,295</span><span class="sxs-lookup"><span data-stu-id="73d35-227">0...4,294,967,295</span></span> |
|                   | <span data-ttu-id="73d35-228">64</span><span class="sxs-lookup"><span data-stu-id="73d35-228">64</span></span>       | `ulong`   | <span data-ttu-id="73d35-229">0...18,446,744,073,709,551,615</span><span class="sxs-lookup"><span data-stu-id="73d35-229">0...18,446,744,073,709,551,615</span></span> |
| <span data-ttu-id="73d35-230">浮点</span><span class="sxs-lookup"><span data-stu-id="73d35-230">Floating point</span></span>    | <span data-ttu-id="73d35-231">32</span><span class="sxs-lookup"><span data-stu-id="73d35-231">32</span></span>       | `float`   | <span data-ttu-id="73d35-232">1.5 × 10 ^-45 到 3.4 × 10 ^38，7 位精度</span><span class="sxs-lookup"><span data-stu-id="73d35-232">1.5 × 10^−45 to 3.4 × 10^38, 7-digit precision</span></span> |
|                   | <span data-ttu-id="73d35-233">64</span><span class="sxs-lookup"><span data-stu-id="73d35-233">64</span></span>       | `double`  | <span data-ttu-id="73d35-234">5.0 × 10 ^-324 到 1.7 × 10 ^308，15 位精度</span><span class="sxs-lookup"><span data-stu-id="73d35-234">5.0 × 10^−324 to 1.7 × 10^308, 15-digit precision</span></span> |
| <span data-ttu-id="73d35-235">十进制</span><span class="sxs-lookup"><span data-stu-id="73d35-235">Decimal</span></span>           | <span data-ttu-id="73d35-236">128</span><span class="sxs-lookup"><span data-stu-id="73d35-236">128</span></span>      | `decimal` | <span data-ttu-id="73d35-237">1.0 × 10 ^28 到 7.9 × 10 ^28、 28 位精度</span><span class="sxs-lookup"><span data-stu-id="73d35-237">1.0 × 10^−28 to 7.9 × 10^28, 28-digit precision</span></span> |

<span data-ttu-id="73d35-238">C# 程序使用***类型声明***创建新类型。</span><span class="sxs-lookup"><span data-stu-id="73d35-238">C# programs use ***type declarations*** to create new types.</span></span> <span data-ttu-id="73d35-239">类型声明指定新类型的名称和成员。</span><span class="sxs-lookup"><span data-stu-id="73d35-239">A type declaration specifies the name and the members of the new type.</span></span> <span data-ttu-id="73d35-240">C# 类型的类别的五个是用户可定义： 类类型、 结构类型、 接口类型、 枚举类型和委托类型。</span><span class="sxs-lookup"><span data-stu-id="73d35-240">Five of C#'s categories of types are user-definable: class types, struct types, interface types, enum types, and delegate types.</span></span>

<span data-ttu-id="73d35-241">类类型定义包含数据成员 （字段） 和函数成员 （方法、 属性和其他人） 的数据结构。</span><span class="sxs-lookup"><span data-stu-id="73d35-241">A class type defines a data structure that contains data members (fields) and function members (methods, properties, and others).</span></span> <span data-ttu-id="73d35-242">类类型支持单一继承和多形性，即派生类可以扩展和专门针对基类的机制。</span><span class="sxs-lookup"><span data-stu-id="73d35-242">Class types support single inheritance and polymorphism, mechanisms whereby derived classes can extend and specialize base classes.</span></span>

<span data-ttu-id="73d35-243">它表示与数据成员和函数成员的结构，结构类型是类类型相似。</span><span class="sxs-lookup"><span data-stu-id="73d35-243">A struct type is similar to a class type in that it represents a structure with data members and function members.</span></span> <span data-ttu-id="73d35-244">但是，与类不同，结构是值类型，不需要堆分配。</span><span class="sxs-lookup"><span data-stu-id="73d35-244">However, unlike classes, structs are value types and do not require heap allocation.</span></span> <span data-ttu-id="73d35-245">结构类型不支持用户指定的继承，并且所有结构类型均隐式继承自类型 `object`。</span><span class="sxs-lookup"><span data-stu-id="73d35-245">Struct types do not support user-specified inheritance, and all struct types implicitly inherit from type `object`.</span></span>

<span data-ttu-id="73d35-246">接口类型作为公共函数成员的命名数据集定义一个协定。</span><span class="sxs-lookup"><span data-stu-id="73d35-246">An interface type defines a contract as a named set of public function members.</span></span> <span data-ttu-id="73d35-247">类或结构实现的接口必须提供接口的函数成员的实现。</span><span class="sxs-lookup"><span data-stu-id="73d35-247">A class or struct that implements an interface must provide implementations of the interface's function members.</span></span> <span data-ttu-id="73d35-248">一个接口可能从多个基接口继承，类或结构可以实现多个接口。</span><span class="sxs-lookup"><span data-stu-id="73d35-248">An interface may inherit from multiple base interfaces, and a class or struct may implement multiple interfaces.</span></span>

<span data-ttu-id="73d35-249">委托类型表示对具有特定参数列表和返回类型的方法的引用。</span><span class="sxs-lookup"><span data-stu-id="73d35-249">A delegate type represents references to methods with a particular parameter list and return type.</span></span> <span data-ttu-id="73d35-250">通过委托，可以将方法视为可分配给变量并可作为参数传递的实体。</span><span class="sxs-lookup"><span data-stu-id="73d35-250">Delegates make it possible to treat methods as entities that can be assigned to variables and passed as parameters.</span></span> <span data-ttu-id="73d35-251">委托类似于其他一些语言中的函数指针概念，但与函数指针不同的是，委托不仅面向对象，还类型安全。</span><span class="sxs-lookup"><span data-stu-id="73d35-251">Delegates are similar to the concept of function pointers found in some other languages, but unlike function pointers, delegates are object-oriented and type-safe.</span></span>

<span data-ttu-id="73d35-252">类、 结构、 接口和委托类型全部都支持泛型，因此它们可以进行参数化与其他类型。</span><span class="sxs-lookup"><span data-stu-id="73d35-252">Class, struct, interface and delegate types all support generics, whereby they can be parameterized with other types.</span></span>

<span data-ttu-id="73d35-253">枚举类型是具有已命名常数的不同类型。</span><span class="sxs-lookup"><span data-stu-id="73d35-253">An enum type is a distinct type with named constants.</span></span> <span data-ttu-id="73d35-254">每个枚举类型都有基础类型，它必须是八种整型类型之一。</span><span class="sxs-lookup"><span data-stu-id="73d35-254">Every enum type has an underlying type, which must be one of the eight integral types.</span></span> <span data-ttu-id="73d35-255">枚举类型的值集是相同的基础类型的值集。</span><span class="sxs-lookup"><span data-stu-id="73d35-255">The set of values of an enum type is the same as the set of values of the underlying type.</span></span>

<span data-ttu-id="73d35-256">C# 支持任意类型的一维和多维数组。</span><span class="sxs-lookup"><span data-stu-id="73d35-256">C# supports single- and multi-dimensional arrays of any type.</span></span> <span data-ttu-id="73d35-257">与上述类型不同，数组类型无需先声明即可使用。</span><span class="sxs-lookup"><span data-stu-id="73d35-257">Unlike the types listed above, array types do not have to be declared before they can be used.</span></span> <span data-ttu-id="73d35-258">相反，数组类型是通过在类型名称后面添加方括号构造而成。</span><span class="sxs-lookup"><span data-stu-id="73d35-258">Instead, array types are constructed by following a type name with square brackets.</span></span> <span data-ttu-id="73d35-259">例如，`int[]`是一维数组`int`，`int[,]`是一个二维数组`int`，并`int[][]`是一维数组的一维数组`int`。</span><span class="sxs-lookup"><span data-stu-id="73d35-259">For example, `int[]` is a single-dimensional array of `int`, `int[,]` is a two-dimensional array of `int`, and `int[][]` is a single-dimensional array of single-dimensional arrays of `int`.</span></span>

<span data-ttu-id="73d35-260">可以为 null 的类型也无需然后可以使用这些声明。</span><span class="sxs-lookup"><span data-stu-id="73d35-260">Nullable types also do not have to be declared before they can be used.</span></span> <span data-ttu-id="73d35-261">对于每个不可为 null 的值类型`T`相应的可以为 null 类型`T?`，后者可以包含其他值`null`。</span><span class="sxs-lookup"><span data-stu-id="73d35-261">For each non-nullable value type `T` there is a corresponding nullable type `T?`, which can hold an additional value `null`.</span></span> <span data-ttu-id="73d35-262">例如，`int?`是可以包含任何 32 位整数或值类型`null`。</span><span class="sxs-lookup"><span data-stu-id="73d35-262">For instance, `int?` is a type that can hold any 32 bit integer or the value `null`.</span></span>

<span data-ttu-id="73d35-263">C# 类型系统被统一的这样可以任何类型的值视为对象。</span><span class="sxs-lookup"><span data-stu-id="73d35-263">C#'s type system is unified such that a value of any type can be treated as an object.</span></span> <span data-ttu-id="73d35-264">每种 C# 类型都直接或间接地派生自 `object` 类类型，而 `object` 是所有类型的最终基类。</span><span class="sxs-lookup"><span data-stu-id="73d35-264">Every type in C# directly or indirectly derives from the `object` class type, and `object` is the ultimate base class of all types.</span></span> <span data-ttu-id="73d35-265">只需将值视为类型 `object`，即可将引用类型的值视为对象。</span><span class="sxs-lookup"><span data-stu-id="73d35-265">Values of reference types are treated as objects simply by viewing the values as type `object`.</span></span> <span data-ttu-id="73d35-266">值类型的值作为对象处理通过执行***装箱***并***取消装箱***操作。</span><span class="sxs-lookup"><span data-stu-id="73d35-266">Values of value types are treated as objects by performing ***boxing*** and ***unboxing*** operations.</span></span> <span data-ttu-id="73d35-267">在以下示例中，`int` 值被转换成 `object`，然后又恢复成 `int`。</span><span class="sxs-lookup"><span data-stu-id="73d35-267">In the following example, an `int` value is converted to `object` and back again to `int`.</span></span>

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
<span data-ttu-id="73d35-268">当一个值类型的值转换为类型`object`、 对象实例，也称为"box"分配为保存值，和的值复制到相应的箱。</span><span class="sxs-lookup"><span data-stu-id="73d35-268">When a value of a value type is converted to type `object`, an object instance, also called a "box," is allocated to hold the value, and the value is copied into that box.</span></span> <span data-ttu-id="73d35-269">相反，当`object`引用强制转换为值类型，引用的对象是正确的值类型的一个框，则进行检查，并检查成功，如果将框中的值复制出来。</span><span class="sxs-lookup"><span data-stu-id="73d35-269">Conversely, when an `object` reference is cast to a value type, a check is made that the referenced object is a box of the correct value type, and, if the check succeeds, the value in the box is copied out.</span></span>

<span data-ttu-id="73d35-270">C# 的统一的类型系统实际上意味着值类型可以转换为"按需。"的对象</span><span class="sxs-lookup"><span data-stu-id="73d35-270">C#'s unified type system effectively means that value types can become objects "on demand."</span></span> <span data-ttu-id="73d35-271">鉴于这种统一性，使用类型 `object` 的常规用途库可以与引用类型和值类型结合使用。</span><span class="sxs-lookup"><span data-stu-id="73d35-271">Because of the unification, general-purpose libraries that use type `object` can be used with both reference types and value types.</span></span>

<span data-ttu-id="73d35-272">C# 有多种***变量***，其中包括字段、数组元素、局部变量和参数。</span><span class="sxs-lookup"><span data-stu-id="73d35-272">There are several kinds of ***variables*** in C#, including fields, array elements, local variables, and parameters.</span></span> <span data-ttu-id="73d35-273">变量表示存储位置，并且每个变量类型，用于确定值可以是存储在变量中，按下表所示。</span><span class="sxs-lookup"><span data-stu-id="73d35-273">Variables represent storage locations, and every variable has a type that determines what values can be stored in the variable, as shown by the following table.</span></span>


| <span data-ttu-id="73d35-274">__变量的类型__</span><span class="sxs-lookup"><span data-stu-id="73d35-274">__Type of Variable__</span></span>    | <span data-ttu-id="73d35-275">__可能的内容__</span><span class="sxs-lookup"><span data-stu-id="73d35-275">__Possible Contents__</span></span> |
|-------------------------|-----------------------|
| <span data-ttu-id="73d35-276">不可以为 null 的值类型</span><span class="sxs-lookup"><span data-stu-id="73d35-276">Non-nullable value type</span></span> | <span data-ttu-id="73d35-277">具有精确类型的值</span><span class="sxs-lookup"><span data-stu-id="73d35-277">A value of that exact type</span></span> |
| <span data-ttu-id="73d35-278">可以为 null 的值类型</span><span class="sxs-lookup"><span data-stu-id="73d35-278">Nullable value type</span></span>     | <span data-ttu-id="73d35-279">Null 值或精确类型的值</span><span class="sxs-lookup"><span data-stu-id="73d35-279">A null value or a value of that exact type</span></span> |
| `object`                | <span data-ttu-id="73d35-280">空引用、 对任何引用类型的对象的引用或对任何值类型的装箱值的引用</span><span class="sxs-lookup"><span data-stu-id="73d35-280">A null reference, a reference to an object of any reference type, or a reference to a boxed value of any value type</span></span> |
| <span data-ttu-id="73d35-281">类类型</span><span class="sxs-lookup"><span data-stu-id="73d35-281">Class type</span></span>              | <span data-ttu-id="73d35-282">派生自类类型的空引用、 对类类型的实例的引用或对类的实例的引用</span><span class="sxs-lookup"><span data-stu-id="73d35-282">A null reference, a reference to an instance of that class type, or a reference to an instance of a class derived from that class type</span></span> |
| <span data-ttu-id="73d35-283">接口类型</span><span class="sxs-lookup"><span data-stu-id="73d35-283">Interface type</span></span>          | <span data-ttu-id="73d35-284">空引用、 对实现接口类型，类类型的实例的引用或对实现该接口类型的值类型的装箱值的引用</span><span class="sxs-lookup"><span data-stu-id="73d35-284">A null reference, a reference to an instance of a class type that implements that interface type, or a reference to a boxed value of a value type that implements that interface type</span></span> |
| <span data-ttu-id="73d35-285">数组类型</span><span class="sxs-lookup"><span data-stu-id="73d35-285">Array type</span></span>              | <span data-ttu-id="73d35-286">空引用、 对该数组类型的实例的引用或对兼容的数组类型的实例的引用</span><span class="sxs-lookup"><span data-stu-id="73d35-286">A null reference, a reference to an instance of that array type, or a reference to an instance of a compatible array type</span></span> |
| <span data-ttu-id="73d35-287">委托类型</span><span class="sxs-lookup"><span data-stu-id="73d35-287">Delegate type</span></span>           | <span data-ttu-id="73d35-288">Null 引用或对该委托类型的实例的引用</span><span class="sxs-lookup"><span data-stu-id="73d35-288">A null reference or a reference to an instance of that delegate type</span></span> |

## <a name="expressions"></a><span data-ttu-id="73d35-289">表达式</span><span class="sxs-lookup"><span data-stu-id="73d35-289">Expressions</span></span>

<span data-ttu-id="73d35-290">***表达式***是在***操作数***和***运算符***的基础之上构造而成。</span><span class="sxs-lookup"><span data-stu-id="73d35-290">***Expressions*** are constructed from ***operands*** and ***operators***.</span></span> <span data-ttu-id="73d35-291">表达式的运算符指明了向操作数应用的运算。</span><span class="sxs-lookup"><span data-stu-id="73d35-291">The operators of an expression indicate which operations to apply to the operands.</span></span> <span data-ttu-id="73d35-292">运算符的示例包括 `+`、`-`、`*`、`/` 和 `new`。</span><span class="sxs-lookup"><span data-stu-id="73d35-292">Examples of operators include `+`, `-`, `*`, `/`, and `new`.</span></span> <span data-ttu-id="73d35-293">操作数的示例包括文本、字段、局部变量和表达式。</span><span class="sxs-lookup"><span data-stu-id="73d35-293">Examples of operands include literals, fields, local variables, and expressions.</span></span>

<span data-ttu-id="73d35-294">如果表达式包含多个运算符，那么运算符的***优先级***决定了各个运算符的计算顺序。</span><span class="sxs-lookup"><span data-stu-id="73d35-294">When an expression contains multiple operators, the ***precedence*** of the operators controls the order in which the individual operators are evaluated.</span></span> <span data-ttu-id="73d35-295">例如，表达式 `x + y * z` 相当于计算 `x + (y * z)`，因为 `*` 运算符的优先级高于 `+` 运算符。</span><span class="sxs-lookup"><span data-stu-id="73d35-295">For example, the expression `x + y * z` is evaluated as `x + (y * z)` because the `*` operator has higher precedence than the `+` operator.</span></span>

<span data-ttu-id="73d35-296">大多数运算符都可以***重载***。</span><span class="sxs-lookup"><span data-stu-id="73d35-296">Most operators can be ***overloaded***.</span></span> <span data-ttu-id="73d35-297">借助运算符重载，可以为一个或两个操作数为用户定义类或结构类型的运算指定用户定义运算符实现代码。</span><span class="sxs-lookup"><span data-stu-id="73d35-297">Operator overloading permits user-defined operator implementations to be specified for operations where one or both of the operands are of a user-defined class or struct type.</span></span>

<span data-ttu-id="73d35-298">下表总结了 C# 运算符，并列出按优先级从高到低的顺序的运算符类别。</span><span class="sxs-lookup"><span data-stu-id="73d35-298">The following table summarizes C#'s operators, listing the operator categories in order of precedence from highest to lowest.</span></span> <span data-ttu-id="73d35-299">同一类别的运算符的优先级也相同。</span><span class="sxs-lookup"><span data-stu-id="73d35-299">Operators in the same category have equal precedence.</span></span>


| <span data-ttu-id="73d35-300">__类别__</span><span class="sxs-lookup"><span data-stu-id="73d35-300">__Category__</span></span>                     | <span data-ttu-id="73d35-301">__表达式__</span><span class="sxs-lookup"><span data-stu-id="73d35-301">__Expression__</span></span>    | <span data-ttu-id="73d35-302">__说明__</span><span class="sxs-lookup"><span data-stu-id="73d35-302">__Description__</span></span> |
|----------------------------------|-------------------|-----------------|
| <span data-ttu-id="73d35-303">基本</span><span class="sxs-lookup"><span data-stu-id="73d35-303">Primary</span></span>                          | `x.m`             | <span data-ttu-id="73d35-304">成员访问</span><span class="sxs-lookup"><span data-stu-id="73d35-304">Member access</span></span> |
|                                  | `x(...)`          | <span data-ttu-id="73d35-305">方法和委托调用</span><span class="sxs-lookup"><span data-stu-id="73d35-305">Method and delegate invocation</span></span> |
|                                  | `x[...]`          | <span data-ttu-id="73d35-306">数组和索引器访问</span><span class="sxs-lookup"><span data-stu-id="73d35-306">Array and indexer access</span></span> |
|                                  | `x++`             | <span data-ttu-id="73d35-307">后递增</span><span class="sxs-lookup"><span data-stu-id="73d35-307">Post-increment</span></span> |
|                                  | `x--`             | <span data-ttu-id="73d35-308">后递减</span><span class="sxs-lookup"><span data-stu-id="73d35-308">Post-decrement</span></span> |
|                                  | `new T(...)`      | <span data-ttu-id="73d35-309">对象和委托创建</span><span class="sxs-lookup"><span data-stu-id="73d35-309">Object and delegate creation</span></span> |
|                                  | `new T(...){...}` | <span data-ttu-id="73d35-310">使用初始值设定项的对象创建</span><span class="sxs-lookup"><span data-stu-id="73d35-310">Object creation with initializer</span></span> |
|                                  | `new {...}`       | <span data-ttu-id="73d35-311">匿名对象初始值设定项</span><span class="sxs-lookup"><span data-stu-id="73d35-311">Anonymous object initializer</span></span> |
|                                  | `new T[...]`      | <span data-ttu-id="73d35-312">数组创建</span><span class="sxs-lookup"><span data-stu-id="73d35-312">Array creation</span></span> |
|                                  | `typeof(T)`       | <span data-ttu-id="73d35-313">获取`System.Type`对象 `T`</span><span class="sxs-lookup"><span data-stu-id="73d35-313">Obtain `System.Type` object for `T`</span></span> |
|                                  | `checked(x)`      | <span data-ttu-id="73d35-314">在已检查的上下文中计算表达式</span><span class="sxs-lookup"><span data-stu-id="73d35-314">Evaluate expression in checked context</span></span> |
|                                  | `unchecked(x)`    | <span data-ttu-id="73d35-315">在未检查的上下文中计算表达式</span><span class="sxs-lookup"><span data-stu-id="73d35-315">Evaluate expression in unchecked context</span></span> |
|                                  | `default(T)`      | <span data-ttu-id="73d35-316">获取类型的默认值 `T`</span><span class="sxs-lookup"><span data-stu-id="73d35-316">Obtain default value of type `T`</span></span> |
|                                  | `delegate {...}`  | <span data-ttu-id="73d35-317">匿名函数（匿名方法）</span><span class="sxs-lookup"><span data-stu-id="73d35-317">Anonymous function (anonymous method)</span></span> |
| <span data-ttu-id="73d35-318">一元</span><span class="sxs-lookup"><span data-stu-id="73d35-318">Unary</span></span>                            | `+x`              | <span data-ttu-id="73d35-319">标识</span><span class="sxs-lookup"><span data-stu-id="73d35-319">Identity</span></span> |
|                                  | `-x`              | <span data-ttu-id="73d35-320">求反</span><span class="sxs-lookup"><span data-stu-id="73d35-320">Negation</span></span> |
|                                  | `!x`              | <span data-ttu-id="73d35-321">逻辑求反</span><span class="sxs-lookup"><span data-stu-id="73d35-321">Logical negation</span></span> |
|                                  | `~x`              | <span data-ttu-id="73d35-322">按位求反</span><span class="sxs-lookup"><span data-stu-id="73d35-322">Bitwise negation</span></span> |
|                                  | `++x`             | <span data-ttu-id="73d35-323">前递增</span><span class="sxs-lookup"><span data-stu-id="73d35-323">Pre-increment</span></span> |
|                                  | `--x`             | <span data-ttu-id="73d35-324">前递减</span><span class="sxs-lookup"><span data-stu-id="73d35-324">Pre-decrement</span></span> |
|                                  | `(T)x`            | <span data-ttu-id="73d35-325">显式转换`x`类型 `T`</span><span class="sxs-lookup"><span data-stu-id="73d35-325">Explicitly convert `x` to type `T`</span></span> |
|                                  | `await x`         | <span data-ttu-id="73d35-326">以异步方式等待`x`完成</span><span class="sxs-lookup"><span data-stu-id="73d35-326">Asynchronously wait for `x` to complete</span></span> |
| <span data-ttu-id="73d35-327">乘法</span><span class="sxs-lookup"><span data-stu-id="73d35-327">Multiplicative</span></span>                   | `x * y`           | <span data-ttu-id="73d35-328">乘法</span><span class="sxs-lookup"><span data-stu-id="73d35-328">Multiplication</span></span> |
|                                  | `x / y`           | <span data-ttu-id="73d35-329">除号</span><span class="sxs-lookup"><span data-stu-id="73d35-329">Division</span></span> |
|                                  | `x % y`           | <span data-ttu-id="73d35-330">余数</span><span class="sxs-lookup"><span data-stu-id="73d35-330">Remainder</span></span> |
| <span data-ttu-id="73d35-331">加法</span><span class="sxs-lookup"><span data-stu-id="73d35-331">Additive</span></span>                         | `x + y`           | <span data-ttu-id="73d35-332">相加、字符串串联、委托组合</span><span class="sxs-lookup"><span data-stu-id="73d35-332">Addition, string concatenation, delegate combination</span></span> |
|                                  | `x - y`           | <span data-ttu-id="73d35-333">相减、委托移除</span><span class="sxs-lookup"><span data-stu-id="73d35-333">Subtraction, delegate removal</span></span> |
| <span data-ttu-id="73d35-334">移位</span><span class="sxs-lookup"><span data-stu-id="73d35-334">Shift</span></span>                            | `x << y`          | <span data-ttu-id="73d35-335">左移</span><span class="sxs-lookup"><span data-stu-id="73d35-335">Shift left</span></span> |
|                                  | `x >> y`          | <span data-ttu-id="73d35-336">右移</span><span class="sxs-lookup"><span data-stu-id="73d35-336">Shift right</span></span> |
| <span data-ttu-id="73d35-337">关系和类型测试</span><span class="sxs-lookup"><span data-stu-id="73d35-337">Relational and type testing</span></span>      | `x < y`           | <span data-ttu-id="73d35-338">小于</span><span class="sxs-lookup"><span data-stu-id="73d35-338">Less than</span></span> |
|                                  | `x > y`           | <span data-ttu-id="73d35-339">大于</span><span class="sxs-lookup"><span data-stu-id="73d35-339">Greater than</span></span> |
|                                  | `x <= y`          | <span data-ttu-id="73d35-340">小于或等于</span><span class="sxs-lookup"><span data-stu-id="73d35-340">Less than or equal</span></span> |
|                                  | `x >= y`          | <span data-ttu-id="73d35-341">大于或等于</span><span class="sxs-lookup"><span data-stu-id="73d35-341">Greater than or equal</span></span> |
|                                  | `x is T`          | <span data-ttu-id="73d35-342">返回`true`如果`x`是`T`，`false`否则为</span><span class="sxs-lookup"><span data-stu-id="73d35-342">Return `true` if `x` is a `T`, `false` otherwise</span></span> |
|                                  | `x as T`          | <span data-ttu-id="73d35-343">返回`x`化为`T`，或`null`如果`x`不是 `T`</span><span class="sxs-lookup"><span data-stu-id="73d35-343">Return `x` typed as `T`, or `null` if `x` is not a `T`</span></span> |
| <span data-ttu-id="73d35-344">相等</span><span class="sxs-lookup"><span data-stu-id="73d35-344">Equality</span></span>                         | `x == y`          | <span data-ttu-id="73d35-345">等于</span><span class="sxs-lookup"><span data-stu-id="73d35-345">Equal</span></span>      |
|                                  | `x != y`          | <span data-ttu-id="73d35-346">不等于</span><span class="sxs-lookup"><span data-stu-id="73d35-346">Not equal</span></span> |
| <span data-ttu-id="73d35-347">逻辑“与”</span><span class="sxs-lookup"><span data-stu-id="73d35-347">Logical AND</span></span>                      | `x & y`           | <span data-ttu-id="73d35-348">整型按位 AND，布尔型逻辑与</span><span class="sxs-lookup"><span data-stu-id="73d35-348">Integer bitwise AND, boolean logical AND</span></span> |
| <span data-ttu-id="73d35-349">逻辑 XOR</span><span class="sxs-lookup"><span data-stu-id="73d35-349">Logical XOR</span></span>                      | `x ^ y`           | <span data-ttu-id="73d35-350">整型按位 XOR，布尔型逻辑 XOR</span><span class="sxs-lookup"><span data-stu-id="73d35-350">Integer bitwise XOR, boolean logical XOR</span></span> |
| <span data-ttu-id="73d35-351">逻辑“或”</span><span class="sxs-lookup"><span data-stu-id="73d35-351">Logical OR</span></span>                       | <code>x &#124; y</code> | <span data-ttu-id="73d35-352">整型按位“或”，布尔型逻辑“或”</span><span class="sxs-lookup"><span data-stu-id="73d35-352">Integer bitwise OR, boolean logical OR</span></span> |
| <span data-ttu-id="73d35-353">条件“与”</span><span class="sxs-lookup"><span data-stu-id="73d35-353">Conditional AND</span></span>                  | `x && y`          | <span data-ttu-id="73d35-354">计算结果`y`仅当`x`是 `true`</span><span class="sxs-lookup"><span data-stu-id="73d35-354">Evaluates `y` only if `x` is `true`</span></span> |
| <span data-ttu-id="73d35-355">条件“或”</span><span class="sxs-lookup"><span data-stu-id="73d35-355">Conditional OR</span></span>                   | <code>x &#124;&#124; y</code> | <span data-ttu-id="73d35-356">计算结果`y`仅当`x`是 `false`</span><span class="sxs-lookup"><span data-stu-id="73d35-356">Evaluates `y` only if `x` is `false`</span></span> |
| <span data-ttu-id="73d35-357">null 合并</span><span class="sxs-lookup"><span data-stu-id="73d35-357">Null coalescing</span></span>                  | `X ?? y`          | <span data-ttu-id="73d35-358">计算结果为`y`如果`x`是`null`到`x`否则为</span><span class="sxs-lookup"><span data-stu-id="73d35-358">Evaluates to `y` if `x` is `null`, to `x` otherwise</span></span> |
| <span data-ttu-id="73d35-359">条件运算</span><span class="sxs-lookup"><span data-stu-id="73d35-359">Conditional</span></span>                      | `x ? y : z`       | <span data-ttu-id="73d35-360">计算结果`y`如果`x`是`true`，`z`如果`x`是 `false`</span><span class="sxs-lookup"><span data-stu-id="73d35-360">Evaluates `y` if `x` is `true`, `z` if `x` is `false`</span></span> |
| <span data-ttu-id="73d35-361">赋值或匿名函数</span><span class="sxs-lookup"><span data-stu-id="73d35-361">Assignment or anonymous function</span></span> | `x = y`           | <span data-ttu-id="73d35-362">赋值</span><span class="sxs-lookup"><span data-stu-id="73d35-362">Assignment</span></span> |
|                                  | `x op= y`         | <span data-ttu-id="73d35-363">复合赋值;支持的运算符是 `*=` `/=` `%=` `+=` `-=` `<<=` `>>=` `&=` `^=` <code>&#124;=</code></span><span class="sxs-lookup"><span data-stu-id="73d35-363">Compound assignment; supported operators are `*=` `/=` `%=` `+=` `-=` `<<=` `>>=` `&=` `^=` <code>&#124;=</code></span></span> |
|                                  | `(T x) => y`      | <span data-ttu-id="73d35-364">匿名函数（lambda 表达式）</span><span class="sxs-lookup"><span data-stu-id="73d35-364">Anonymous function (lambda expression)</span></span> |

## <a name="statements"></a><span data-ttu-id="73d35-365">语句</span><span class="sxs-lookup"><span data-stu-id="73d35-365">Statements</span></span>

<span data-ttu-id="73d35-366">程序操作使用***语句***进行表示。</span><span class="sxs-lookup"><span data-stu-id="73d35-366">The actions of a program are expressed using ***statements***.</span></span> <span data-ttu-id="73d35-367">C# 支持几种不同的语句，其中许多语句是从嵌入语句的角度来定义的。</span><span class="sxs-lookup"><span data-stu-id="73d35-367">C# supports several different kinds of statements, a number of which are defined in terms of embedded statements.</span></span>

<span data-ttu-id="73d35-368">使用***代码块***，可以在允许编写一个语句的上下文中编写多个语句。</span><span class="sxs-lookup"><span data-stu-id="73d35-368">A ***block*** permits multiple statements to be written in contexts where a single statement is allowed.</span></span> <span data-ttu-id="73d35-369">代码块是由一系列在分隔符 `{` 和 `}` 内编写的语句组成。</span><span class="sxs-lookup"><span data-stu-id="73d35-369">A block consists of a list of statements written between the delimiters `{` and `}`.</span></span>

<span data-ttu-id="73d35-370">***声明语句***用于声明局部变量和常量。</span><span class="sxs-lookup"><span data-stu-id="73d35-370">***Declaration statements*** are used to declare local variables and constants.</span></span>

<span data-ttu-id="73d35-371">***表达式语句***用于计算表达式。</span><span class="sxs-lookup"><span data-stu-id="73d35-371">***Expression statements*** are used to evaluate expressions.</span></span> <span data-ttu-id="73d35-372">可用作语句的表达式包括方法调用的对象使用的分配`new`运算符、 角色分配使用`=`和复合赋值运算符，使用递增和递减操作`++`和`--`运算符和 await 表达式。</span><span class="sxs-lookup"><span data-stu-id="73d35-372">Expressions that can be used as statements include method invocations, object allocations using the `new` operator, assignments using `=` and the compound assignment operators, increment and decrement operations using the `++` and `--` operators and await expressions.</span></span>

<span data-ttu-id="73d35-373">***选择语句***用于根据一些表达式的值从多个可能的语句中选择一个以供执行。</span><span class="sxs-lookup"><span data-stu-id="73d35-373">***Selection statements*** are used to select one of a number of possible statements for execution based on the value of some expression.</span></span> <span data-ttu-id="73d35-374">这一类语句包括 `if` 和 `switch` 语句。</span><span class="sxs-lookup"><span data-stu-id="73d35-374">In this group are the `if` and `switch` statements.</span></span>

<span data-ttu-id="73d35-375">***迭代语句***用于重复执行嵌入的语句。</span><span class="sxs-lookup"><span data-stu-id="73d35-375">***Iteration statements*** are used to repeatedly execute an embedded statement.</span></span> <span data-ttu-id="73d35-376">这一类语句包括 `while`、`do`、`for` 和 `foreach` 语句。</span><span class="sxs-lookup"><span data-stu-id="73d35-376">In this group are the `while`, `do`, `for`, and `foreach` statements.</span></span>

<span data-ttu-id="73d35-377">***跳转语句***用于转移控制权。</span><span class="sxs-lookup"><span data-stu-id="73d35-377">***Jump statements*** are used to transfer control.</span></span> <span data-ttu-id="73d35-378">这一类语句包括 `break`、`continue`、`goto`、`throw`、`return` 和 `yield` 语句。</span><span class="sxs-lookup"><span data-stu-id="73d35-378">In this group are the `break`, `continue`, `goto`, `throw`, `return`, and `yield` statements.</span></span>

<span data-ttu-id="73d35-379">`try`...`catch` 语句用于捕获在代码块执行期间发生的异常，`try`...`finally` 语句用于指定始终执行的最终代码，无论异常发生与否。</span><span class="sxs-lookup"><span data-stu-id="73d35-379">The `try`...`catch` statement is used to catch exceptions that occur during execution of a block, and the `try`...`finally` statement is used to specify finalization code that is always executed, whether an exception occurred or not.</span></span>

<span data-ttu-id="73d35-380">`checked`和`unchecked`语句用于控制溢出检查上下文的整型类型算术运算和转换。</span><span class="sxs-lookup"><span data-stu-id="73d35-380">The `checked` and `unchecked` statements are used to control the overflow checking context for integral-type arithmetic operations and conversions.</span></span>

<span data-ttu-id="73d35-381">`lock` 语句用于获取给定对象的相互排斥锁定，执行语句，然后解除锁定。</span><span class="sxs-lookup"><span data-stu-id="73d35-381">The `lock` statement is used to obtain the mutual-exclusion lock for a given object, execute a statement, and then release the lock.</span></span>

<span data-ttu-id="73d35-382">`using` 语句用于获取资源，执行语句，然后释放资源。</span><span class="sxs-lookup"><span data-stu-id="73d35-382">The `using` statement is used to obtain a resource, execute a statement, and then dispose of that resource.</span></span>

<span data-ttu-id="73d35-383">下面是语句的每个类型示例</span><span class="sxs-lookup"><span data-stu-id="73d35-383">Below are examples of each kind of statement</span></span>

<span data-ttu-id="73d35-384">__本地变量声明__</span><span class="sxs-lookup"><span data-stu-id="73d35-384">__Local variable declarations__</span></span>

```csharp
static void Main() {
   int a;
   int b = 2, c = 3;
   a = 1;
   Console.WriteLine(a + b + c);
}
```


<span data-ttu-id="73d35-385">__局部常量声明__</span><span class="sxs-lookup"><span data-stu-id="73d35-385">__Local constant declaration__</span></span>

```csharp
static void Main() {
    const float pi = 3.1415927f;
    const int r = 25;
    Console.WriteLine(pi * r * r);
}
```


<span data-ttu-id="73d35-386">__表达式语句__</span><span class="sxs-lookup"><span data-stu-id="73d35-386">__Expression statement__</span></span>

```csharp
static void Main() {
    int i;
    i = 123;                // Expression statement
    Console.WriteLine(i);   // Expression statement
    i++;                    // Expression statement
    Console.WriteLine(i);   // Expression statement
}
```

<span data-ttu-id="73d35-387">__`if` 语句__</span><span class="sxs-lookup"><span data-stu-id="73d35-387">__`if` statement__</span></span>

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


<span data-ttu-id="73d35-388">__`switch` 语句__</span><span class="sxs-lookup"><span data-stu-id="73d35-388">__`switch` statement__</span></span>

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

<span data-ttu-id="73d35-389">__`while` 语句__</span><span class="sxs-lookup"><span data-stu-id="73d35-389">__`while` statement__</span></span>

```csharp
static void Main(string[] args) {
    int i = 0;
    while (i < args.Length) {
        Console.WriteLine(args[i]);
        i++;
    }
}
```


<span data-ttu-id="73d35-390">__`do` 语句__</span><span class="sxs-lookup"><span data-stu-id="73d35-390">__`do` statement__</span></span>

```csharp
static void Main() {
    string s;
    do {
        s = Console.ReadLine();
        if (s != null) Console.WriteLine(s);
    } while (s != null);
}
```

<span data-ttu-id="73d35-391">__`for` 语句__</span><span class="sxs-lookup"><span data-stu-id="73d35-391">__`for` statement__</span></span>

```csharp
static void Main(string[] args) {
    for (int i = 0; i < args.Length; i++) {
        Console.WriteLine(args[i]);
    }
}
```

<span data-ttu-id="73d35-392">__`foreach` 语句__</span><span class="sxs-lookup"><span data-stu-id="73d35-392">__`foreach` statement__</span></span>

```csharp
static void Main(string[] args) {
    foreach (string s in args) {
        Console.WriteLine(s);
    }
}
```

<span data-ttu-id="73d35-393">__`break` 语句__</span><span class="sxs-lookup"><span data-stu-id="73d35-393">__`break` statement__</span></span>

```csharp
static void Main() {
    while (true) {
        string s = Console.ReadLine();
        if (s == null) break;
        Console.WriteLine(s);
    }
}
```

<span data-ttu-id="73d35-394">__`continue` 语句__</span><span class="sxs-lookup"><span data-stu-id="73d35-394">__`continue` statement__</span></span>

```csharp
static void Main(string[] args) {
    for (int i = 0; i < args.Length; i++) {
        if (args[i].StartsWith("/")) continue;
        Console.WriteLine(args[i]);
    }
}
```

<span data-ttu-id="73d35-395">__`goto` 语句__</span><span class="sxs-lookup"><span data-stu-id="73d35-395">__`goto` statement__</span></span>

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

<span data-ttu-id="73d35-396">__`return` 语句__</span><span class="sxs-lookup"><span data-stu-id="73d35-396">__`return` statement__</span></span>

```csharp
static int Add(int a, int b) {
    return a + b;
}

static void Main() {
    Console.WriteLine(Add(1, 2));
    return;
}
```

<span data-ttu-id="73d35-397">__`yield` 语句__</span><span class="sxs-lookup"><span data-stu-id="73d35-397">__`yield` statement__</span></span>

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

<span data-ttu-id="73d35-398">__`throw` 和`try`语句__</span><span class="sxs-lookup"><span data-stu-id="73d35-398">__`throw` and `try` statements__</span></span>

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

<span data-ttu-id="73d35-399">__`checked` 和`unchecked`语句__</span><span class="sxs-lookup"><span data-stu-id="73d35-399">__`checked` and `unchecked` statements__</span></span>

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

<span data-ttu-id="73d35-400">__`lock` 语句__</span><span class="sxs-lookup"><span data-stu-id="73d35-400">__`lock` statement__</span></span>

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

<span data-ttu-id="73d35-401">__`using` 语句__</span><span class="sxs-lookup"><span data-stu-id="73d35-401">__`using` statement__</span></span>

```csharp
static void Main() {
    using (TextWriter w = File.CreateText("test.txt")) {
        w.WriteLine("Line one");
        w.WriteLine("Line two");
        w.WriteLine("Line three");
    }
}
```

## <a name="classes-and-objects"></a><span data-ttu-id="73d35-402">类和对象</span><span class="sxs-lookup"><span data-stu-id="73d35-402">Classes and objects</span></span>

<span data-ttu-id="73d35-403">***类***是最基本的 C# 类型。</span><span class="sxs-lookup"><span data-stu-id="73d35-403">***Classes*** are the most fundamental of C#'s types.</span></span> <span data-ttu-id="73d35-404">类是一种数据结构，可在一个单元中就将状态（字段）和操作（方法和其他函数成员）结合起来。</span><span class="sxs-lookup"><span data-stu-id="73d35-404">A class is a data structure that combines state (fields) and actions (methods and other function members) in a single unit.</span></span> <span data-ttu-id="73d35-405">类为动态创建的类***实例***（亦称为“***对象***”）提供了定义。</span><span class="sxs-lookup"><span data-stu-id="73d35-405">A class provides a definition for dynamically created ***instances*** of the class, also known as ***objects***.</span></span> <span data-ttu-id="73d35-406">类支持***继承***和***多形性***，即***派生类***可以扩展和专门针对***基类***的机制。</span><span class="sxs-lookup"><span data-stu-id="73d35-406">Classes support ***inheritance*** and ***polymorphism***, mechanisms whereby ***derived classes*** can extend and specialize ***base classes***.</span></span>

<span data-ttu-id="73d35-407">新类使用类声明进行创建。</span><span class="sxs-lookup"><span data-stu-id="73d35-407">New classes are created using class declarations.</span></span> <span data-ttu-id="73d35-408">类声明的开头是标头，指定了类的特性和修饰符、类名、基类（若指定）以及类实现的接口。</span><span class="sxs-lookup"><span data-stu-id="73d35-408">A class declaration starts with a header that specifies the attributes and modifiers of the class, the name of the class, the base class (if given), and the interfaces implemented by the class.</span></span> <span data-ttu-id="73d35-409">标头后面是类主体，由在分隔符 `{` 和 `}` 内编写的成员声明列表组成。</span><span class="sxs-lookup"><span data-stu-id="73d35-409">The header is followed by the class body, which consists of a list of member declarations written between the delimiters `{` and `}`.</span></span>

<span data-ttu-id="73d35-410">以下是简单类 `Point` 的声明：</span><span class="sxs-lookup"><span data-stu-id="73d35-410">The following is a declaration of a simple class named `Point`:</span></span>

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
<span data-ttu-id="73d35-411">类实例是使用 `new` 运算符进行创建，此运算符为新实例分配内存，调用构造函数来初始化实例，并返回对实例的引用。</span><span class="sxs-lookup"><span data-stu-id="73d35-411">Instances of classes are created using the `new` operator, which allocates memory for a new instance, invokes a constructor to initialize the instance, and returns a reference to the instance.</span></span> <span data-ttu-id="73d35-412">以下语句创建两个`Point`对象并将对这些对象的引用存储在两个变量：</span><span class="sxs-lookup"><span data-stu-id="73d35-412">The following statements create two `Point` objects and store references to those objects in two variables:</span></span>

```
Point p1 = new Point(0, 0);
Point p2 = new Point(10, 20);
```
<span data-ttu-id="73d35-413">不再使用对象时，将自动收回由对象占用的内存。</span><span class="sxs-lookup"><span data-stu-id="73d35-413">The memory occupied by an object is automatically reclaimed when the object is no longer in use.</span></span> <span data-ttu-id="73d35-414">既没必要，也无法在 C# 中显式解除分配对象。</span><span class="sxs-lookup"><span data-stu-id="73d35-414">It is neither necessary nor possible to explicitly deallocate objects in C#.</span></span>

### <a name="members"></a><span data-ttu-id="73d35-415">成员</span><span class="sxs-lookup"><span data-stu-id="73d35-415">Members</span></span>

<span data-ttu-id="73d35-416">类的成员为***静态成员***或***实例成员***。</span><span class="sxs-lookup"><span data-stu-id="73d35-416">The members of a class are either ***static members*** or ***instance members***.</span></span> <span data-ttu-id="73d35-417">静态成员属于类，而实例成员则属于对象（类实例）。</span><span class="sxs-lookup"><span data-stu-id="73d35-417">Static members belong to classes, and instance members belong to objects (instances of classes).</span></span>

<span data-ttu-id="73d35-418">下表提供了一个类可以包含的成员类型的概述。</span><span class="sxs-lookup"><span data-stu-id="73d35-418">The following table provides an overview of the kinds of members a class can contain.</span></span>


| <span data-ttu-id="73d35-419">__成员__</span><span class="sxs-lookup"><span data-stu-id="73d35-419">__Member__</span></span>   | <span data-ttu-id="73d35-420">__说明__</span><span class="sxs-lookup"><span data-stu-id="73d35-420">__Description__</span></span> |
|------------  |-----------------|
| <span data-ttu-id="73d35-421">常量</span><span class="sxs-lookup"><span data-stu-id="73d35-421">Constants</span></span>    | <span data-ttu-id="73d35-422">与类相关联的常量值</span><span class="sxs-lookup"><span data-stu-id="73d35-422">Constant values associated with the class</span></span> |
| <span data-ttu-id="73d35-423">字段</span><span class="sxs-lookup"><span data-stu-id="73d35-423">Fields</span></span>       | <span data-ttu-id="73d35-424">类的常量</span><span class="sxs-lookup"><span data-stu-id="73d35-424">Variables of the class</span></span> |
| <span data-ttu-id="73d35-425">方法</span><span class="sxs-lookup"><span data-stu-id="73d35-425">Methods</span></span>      | <span data-ttu-id="73d35-426">类可以执行的计算和操作</span><span class="sxs-lookup"><span data-stu-id="73d35-426">Computations and actions that can be performed by the class</span></span> |
| <span data-ttu-id="73d35-427">属性</span><span class="sxs-lookup"><span data-stu-id="73d35-427">Properties</span></span>   | <span data-ttu-id="73d35-428">与读取和写入类的已命名属性相关联的操作</span><span class="sxs-lookup"><span data-stu-id="73d35-428">Actions associated with reading and writing named properties of the class</span></span> |
| <span data-ttu-id="73d35-429">索引器</span><span class="sxs-lookup"><span data-stu-id="73d35-429">Indexers</span></span>     | <span data-ttu-id="73d35-430">与将类实例编入索引（像处理数组一样）相关联的操作</span><span class="sxs-lookup"><span data-stu-id="73d35-430">Actions associated with indexing instances of the class like an array</span></span> |
| <span data-ttu-id="73d35-431">事件</span><span class="sxs-lookup"><span data-stu-id="73d35-431">Events</span></span>       | <span data-ttu-id="73d35-432">类可以生成的通知</span><span class="sxs-lookup"><span data-stu-id="73d35-432">Notifications that can be generated by the class</span></span> |
| <span data-ttu-id="73d35-433">运算符</span><span class="sxs-lookup"><span data-stu-id="73d35-433">Operators</span></span>    | <span data-ttu-id="73d35-434">类支持的转换和表达式运算符</span><span class="sxs-lookup"><span data-stu-id="73d35-434">Conversions and expression operators supported by the class</span></span> |
| <span data-ttu-id="73d35-435">构造函数</span><span class="sxs-lookup"><span data-stu-id="73d35-435">Constructors</span></span> | <span data-ttu-id="73d35-436">初始化类实例或类本身所需的操作</span><span class="sxs-lookup"><span data-stu-id="73d35-436">Actions required to initialize instances of the class or the class itself</span></span> |
| <span data-ttu-id="73d35-437">析构函数</span><span class="sxs-lookup"><span data-stu-id="73d35-437">Destructors</span></span>  | <span data-ttu-id="73d35-438">永久放弃类实例前要执行的操作</span><span class="sxs-lookup"><span data-stu-id="73d35-438">Actions to perform before instances of the class are permanently discarded</span></span> |
| <span data-ttu-id="73d35-439">类型</span><span class="sxs-lookup"><span data-stu-id="73d35-439">Types</span></span>        | <span data-ttu-id="73d35-440">类声明的嵌套类型</span><span class="sxs-lookup"><span data-stu-id="73d35-440">Nested types declared by the class</span></span> |

### <a name="accessibility"></a><span data-ttu-id="73d35-441">可访问性</span><span class="sxs-lookup"><span data-stu-id="73d35-441">Accessibility</span></span>

<span data-ttu-id="73d35-442">每个类成员都有关联的可访问性，用于控制能够访问成员的程序文本区域。</span><span class="sxs-lookup"><span data-stu-id="73d35-442">Each member of a class has an associated accessibility, which controls the regions of program text that are able to access the member.</span></span> <span data-ttu-id="73d35-443">可访问性有五种可能的形式。</span><span class="sxs-lookup"><span data-stu-id="73d35-443">There are five possible forms of accessibility.</span></span> <span data-ttu-id="73d35-444">下表概述了这些报表。</span><span class="sxs-lookup"><span data-stu-id="73d35-444">These are summarized in the following table.</span></span>


| <span data-ttu-id="73d35-445">__辅助功能__</span><span class="sxs-lookup"><span data-stu-id="73d35-445">__Accessibility__</span></span>    | <span data-ttu-id="73d35-446">__含义__</span><span class="sxs-lookup"><span data-stu-id="73d35-446">__Meaning__</span></span> |
|----------------------|-----------------|
| `public`             | <span data-ttu-id="73d35-447">访问不受限</span><span class="sxs-lookup"><span data-stu-id="73d35-447">Access not limited</span></span> |
| `protected`          | <span data-ttu-id="73d35-448">只能访问此类或派生自此类的类</span><span class="sxs-lookup"><span data-stu-id="73d35-448">Access limited to this class or classes derived from this class</span></span> |
| `internal`           | <span data-ttu-id="73d35-449">只能访问此程序</span><span class="sxs-lookup"><span data-stu-id="73d35-449">Access limited to this program</span></span> |
| `protected internal` | <span data-ttu-id="73d35-450">只能访问此程序或派生自此类的类</span><span class="sxs-lookup"><span data-stu-id="73d35-450">Access limited to this program or classes derived from this class</span></span> |
| `private`            | <span data-ttu-id="73d35-451">只能访问此类</span><span class="sxs-lookup"><span data-stu-id="73d35-451">Access limited to this class</span></span> |

### <a name="type-parameters"></a><span data-ttu-id="73d35-452">类型参数</span><span class="sxs-lookup"><span data-stu-id="73d35-452">Type parameters</span></span>

<span data-ttu-id="73d35-453">类定义可能会按如下方式指定一组类型参数：在类名后面用尖括号括住类型参数名称列表。</span><span class="sxs-lookup"><span data-stu-id="73d35-453">A class definition may specify a set of type parameters by following the class name with angle brackets enclosing a list of type parameter names.</span></span> <span data-ttu-id="73d35-454">类型参数可用于在类声明的主体中定义类的成员。</span><span class="sxs-lookup"><span data-stu-id="73d35-454">The type parameters can the be used in the body of the class declarations to define the members of the class.</span></span> <span data-ttu-id="73d35-455">在以下示例中，`Pair` 的类型参数是 `TFirst` 和 `TSecond`：</span><span class="sxs-lookup"><span data-stu-id="73d35-455">In the following example, the type parameters of `Pair` are `TFirst` and `TSecond`:</span></span>

```csharp
public class Pair<TFirst,TSecond>
{
    public TFirst First;
    public TSecond Second;
}
```
<span data-ttu-id="73d35-456">被声明为采用类型参数的类类型称为泛型类类型。</span><span class="sxs-lookup"><span data-stu-id="73d35-456">A class type that is declared to take type parameters is called a generic class type.</span></span> <span data-ttu-id="73d35-457">结构、接口和委托类型也可以是泛型。</span><span class="sxs-lookup"><span data-stu-id="73d35-457">Struct, interface and delegate types can also be generic.</span></span>

<span data-ttu-id="73d35-458">使用泛型类时，必须为每个类型参数提供类型自变量：</span><span class="sxs-lookup"><span data-stu-id="73d35-458">When the generic class is used, type arguments must be provided for each of the type parameters:</span></span>

```csharp
Pair<int,string> pair = new Pair<int,string> { First = 1, Second = "two" };
int i = pair.First;     // TFirst is int
string s = pair.Second; // TSecond is string
```
<span data-ttu-id="73d35-459">泛型类型包含类型自变量，如`Pair<int,string>
    `更高版本，称为构造的类型。</span><span class="sxs-lookup"><span data-stu-id="73d35-459">A generic type with type arguments provided, like `Pair<int,string>
    ` above, is called a constructed type.</span></span>

### <a name="base-classes"></a><span data-ttu-id="73d35-460">基类</span><span class="sxs-lookup"><span data-stu-id="73d35-460">Base classes</span></span>

<span data-ttu-id="73d35-461">类声明可能会按如下方式指定基类：在类名和类型参数后面编写冒号和基类名。</span><span class="sxs-lookup"><span data-stu-id="73d35-461">A class declaration may specify a base class by following the class name and type parameters with a colon and the name of the base class.</span></span> <span data-ttu-id="73d35-462">省略基类规范与从 `object` 类型派生相同。</span><span class="sxs-lookup"><span data-stu-id="73d35-462">Omitting a base class specification is the same as deriving from type `object`.</span></span> <span data-ttu-id="73d35-463">在以下示例中，`Point3D` 的基类是 `Point`，`Point` 的基类是 `object`：</span><span class="sxs-lookup"><span data-stu-id="73d35-463">In the following example, the base class of `Point3D` is `Point`, and the base class of `Point` is `object`:</span></span>

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
<span data-ttu-id="73d35-464">类继承其基类的成员。</span><span class="sxs-lookup"><span data-stu-id="73d35-464">A class inherits the members of its base class.</span></span> <span data-ttu-id="73d35-465">继承是指一个类隐式包含其基本类，实例和静态构造函数和基类的析构函数除外的所有成员。</span><span class="sxs-lookup"><span data-stu-id="73d35-465">Inheritance means that a class implicitly contains all members of its base class, except for the instance and static constructors, and the destructors of the base class.</span></span> <span data-ttu-id="73d35-466">派生类可以其继承的类添加新成员，但无法删除继承成员的定义。</span><span class="sxs-lookup"><span data-stu-id="73d35-466">A derived class can add new members to those it inherits, but it cannot remove the definition of an inherited member.</span></span> <span data-ttu-id="73d35-467">在上面的示例中，`Point3D` 从 `Point` 继承了 `x` 和 `y` 字段，每个 `Point3D` 实例均包含三个字段（`x`、`y` 和 `z`）。</span><span class="sxs-lookup"><span data-stu-id="73d35-467">In the previous example, `Point3D` inherits the `x` and `y` fields from `Point`, and every `Point3D` instance contains three fields, `x`, `y`, and `z`.</span></span>

<span data-ttu-id="73d35-468">可以将类类型隐式转换成其任意基类类型。</span><span class="sxs-lookup"><span data-stu-id="73d35-468">An implicit conversion exists from a class type to any of its base class types.</span></span> <span data-ttu-id="73d35-469">因此，类类型的变量可以引用相应类的实例或任意派生类的实例。</span><span class="sxs-lookup"><span data-stu-id="73d35-469">Therefore, a variable of a class type can reference an instance of that class or an instance of any derived class.</span></span> <span data-ttu-id="73d35-470">例如，类声明如上，`Point` 类型的变量可以引用 `Point` 或 `Point3D`：</span><span class="sxs-lookup"><span data-stu-id="73d35-470">For example, given the previous class declarations, a variable of type `Point` can reference either a `Point` or a `Point3D`:</span></span>

```csharp
Point a = new Point(10, 20);
Point b = new Point3D(10, 20, 30);
```

### <a name="fields"></a><span data-ttu-id="73d35-471">字段</span><span class="sxs-lookup"><span data-stu-id="73d35-471">Fields</span></span>

<span data-ttu-id="73d35-472">字段是一个类或类的实例相关联的变量。</span><span class="sxs-lookup"><span data-stu-id="73d35-472">A field is a variable that is associated with a class or with an instance of a class.</span></span>

<span data-ttu-id="73d35-473">使用字段声明`static`修饰符定义***静态字段***。</span><span class="sxs-lookup"><span data-stu-id="73d35-473">A field declared with the `static` modifier defines a ***static field***.</span></span> <span data-ttu-id="73d35-474">静态字段只指明一个存储位置。</span><span class="sxs-lookup"><span data-stu-id="73d35-474">A static field identifies exactly one storage location.</span></span> <span data-ttu-id="73d35-475">无论创建多少个类实例，永远只有一个静态字段副本。</span><span class="sxs-lookup"><span data-stu-id="73d35-475">No matter how many instances of a class are created, there is only ever one copy of a static field.</span></span>

<span data-ttu-id="73d35-476">字段声明而无需`static`修饰符定义***实例字段***。</span><span class="sxs-lookup"><span data-stu-id="73d35-476">A field declared without the `static` modifier defines an ***instance field***.</span></span> <span data-ttu-id="73d35-477">每个类实例均包含相应类的所有实例字段的单独副本。</span><span class="sxs-lookup"><span data-stu-id="73d35-477">Every instance of a class contains a separate copy of all the instance fields of that class.</span></span>

<span data-ttu-id="73d35-478">在以下示例中，每个 `Color` 类实例均包含 `r`、`g` 和 `b` 实例字段的单独副本，但分别只包含 `Black`、`White`、`Red`、`Green` 和 `Blue` 静态字段的一个副本：</span><span class="sxs-lookup"><span data-stu-id="73d35-478">In the following example, each instance of the `Color` class has a separate copy of the `r`, `g`, and `b` instance fields, but there is only one copy of the `Black`, `White`, `Red`, `Green`, and `Blue` static fields:</span></span>

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
<span data-ttu-id="73d35-479">如上面的示例所示，可以使用 `readonly` 修饰符声明***只读字段***。</span><span class="sxs-lookup"><span data-stu-id="73d35-479">As shown in the previous example, ***read-only fields*** may be declared with a `readonly` modifier.</span></span> <span data-ttu-id="73d35-480">分配给`readonly`字段仅可用作字段的声明或同一个类的构造函数中。</span><span class="sxs-lookup"><span data-stu-id="73d35-480">Assignment to a `readonly` field can only occur as part of the field's declaration or in a constructor in the same class.</span></span>

### <a name="methods"></a><span data-ttu-id="73d35-481">方法</span><span class="sxs-lookup"><span data-stu-id="73d35-481">Methods</span></span>

<span data-ttu-id="73d35-482">***方法***是实现对象或类可执行的计算或操作的成员。</span><span class="sxs-lookup"><span data-stu-id="73d35-482">A ***method*** is a member that implements a computation or action that can be performed by an object or class.</span></span> <span data-ttu-id="73d35-483">***静态方法***是通过类进行访问。</span><span class="sxs-lookup"><span data-stu-id="73d35-483">***Static methods*** are accessed through the class.</span></span> <span data-ttu-id="73d35-484">***实例方法***是通过类实例进行访问。</span><span class="sxs-lookup"><span data-stu-id="73d35-484">***Instance methods*** are accessed through instances of the class.</span></span>

<span data-ttu-id="73d35-485">方法有一个 （可能为空） 的列表***参数***，分别代表值或变量引用传递给方法，和一个***返回类型***，它指定计算并返回值的类型该方法。</span><span class="sxs-lookup"><span data-stu-id="73d35-485">Methods have a (possibly empty) list of ***parameters***, which represent values or variable references passed to the method, and a ***return type***, which specifies the type of the value computed and returned by the method.</span></span> <span data-ttu-id="73d35-486">方法的返回类型是`void`如果它不返回值。</span><span class="sxs-lookup"><span data-stu-id="73d35-486">A method's return type is `void` if it does not return a value.</span></span>

<span data-ttu-id="73d35-487">方法可能也包含一组类型参数，必须在调用方法时指定类型自变量，这一点与类型一样。</span><span class="sxs-lookup"><span data-stu-id="73d35-487">Like types, methods may also have a set of type parameters, for which type arguments must be specified when the method is called.</span></span> <span data-ttu-id="73d35-488">与类型不同的是，通常可以根据方法调用的自变量推断出类型自变量，无需显式指定。</span><span class="sxs-lookup"><span data-stu-id="73d35-488">Unlike types, the type arguments can often be inferred from the arguments of a method call and need not be explicitly given.</span></span>

<span data-ttu-id="73d35-489">在声明方法的类中，方法的***签名***必须是唯一的。</span><span class="sxs-lookup"><span data-stu-id="73d35-489">The ***signature*** of a method must be unique in the class in which the method is declared.</span></span> <span data-ttu-id="73d35-490">方法签名包含方法名称、类型参数数量及其参数的数量、修饰符和类型。</span><span class="sxs-lookup"><span data-stu-id="73d35-490">The signature of a method consists of the name of the method, the number of type parameters and the number, modifiers, and types of its parameters.</span></span> <span data-ttu-id="73d35-491">方法签名不包含返回类型。</span><span class="sxs-lookup"><span data-stu-id="73d35-491">The signature of a method does not include the return type.</span></span>

#### <a name="parameters"></a><span data-ttu-id="73d35-492">参数</span><span class="sxs-lookup"><span data-stu-id="73d35-492">Parameters</span></span>

<span data-ttu-id="73d35-493">参数用于将值或变量引用传递给方法。</span><span class="sxs-lookup"><span data-stu-id="73d35-493">Parameters are used to pass values or variable references to methods.</span></span> <span data-ttu-id="73d35-494">方法参数从调用方法时指定的***自变量***中获取其实际值。</span><span class="sxs-lookup"><span data-stu-id="73d35-494">The parameters of a method get their actual values from the ***arguments*** that are specified when the method is invoked.</span></span> <span data-ttu-id="73d35-495">有四类参数：值参数、引用参数、输出参数和参数数组。</span><span class="sxs-lookup"><span data-stu-id="73d35-495">There are four kinds of parameters: value parameters, reference parameters, output parameters, and parameter arrays.</span></span>

<span data-ttu-id="73d35-496">***值参数***用于传递输入参数。</span><span class="sxs-lookup"><span data-stu-id="73d35-496">A ***value parameter*** is used for input parameter passing.</span></span> <span data-ttu-id="73d35-497">值参数对应于局部变量，从为其传递的自变量中获取初始值。</span><span class="sxs-lookup"><span data-stu-id="73d35-497">A value parameter corresponds to a local variable that gets its initial value from the argument that was passed for the parameter.</span></span> <span data-ttu-id="73d35-498">修改值参数不会影响为其传递的自变量。</span><span class="sxs-lookup"><span data-stu-id="73d35-498">Modifications to a value parameter do not affect the argument that was passed for the parameter.</span></span>

<span data-ttu-id="73d35-499">可以指定默认值，从而省略相应的自变量，这样值参数就是可选的。</span><span class="sxs-lookup"><span data-stu-id="73d35-499">Value parameters can be optional, by specifying a default value so that corresponding arguments can be omitted.</span></span>

<span data-ttu-id="73d35-500">***引用参数***用于传递输入和输出参数。</span><span class="sxs-lookup"><span data-stu-id="73d35-500">A ***reference parameter*** is used for both input and output parameter passing.</span></span> <span data-ttu-id="73d35-501">为引用参数传递的自变量必须是变量，并且在方法执行期间，引用参数指明的存储位置与自变量相同。</span><span class="sxs-lookup"><span data-stu-id="73d35-501">The argument passed for a reference parameter must be a variable, and during execution of the method, the reference parameter represents the same storage location as the argument variable.</span></span> <span data-ttu-id="73d35-502">引用参数使用 `ref` 修饰符进行声明。</span><span class="sxs-lookup"><span data-stu-id="73d35-502">A reference parameter is declared with the `ref` modifier.</span></span> <span data-ttu-id="73d35-503">下面的示例展示了如何使用 `ref` 参数。</span><span class="sxs-lookup"><span data-stu-id="73d35-503">The following example shows the use of `ref` parameters.</span></span>

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
<span data-ttu-id="73d35-504">***输出参数***用于传递输出参数。</span><span class="sxs-lookup"><span data-stu-id="73d35-504">An ***output parameter*** is used for output parameter passing.</span></span> <span data-ttu-id="73d35-505">输出参数与引用参数类似，不同之处在于，调用方提供的自变量的初始值并不重要。</span><span class="sxs-lookup"><span data-stu-id="73d35-505">An output parameter is similar to a reference parameter except that the initial value of the caller-provided argument is unimportant.</span></span> <span data-ttu-id="73d35-506">输出参数使用 `out` 修饰符进行声明。</span><span class="sxs-lookup"><span data-stu-id="73d35-506">An output parameter is declared with the `out` modifier.</span></span> <span data-ttu-id="73d35-507">下面的示例展示了如何使用 `out` 参数。</span><span class="sxs-lookup"><span data-stu-id="73d35-507">The following example shows the use of `out` parameters.</span></span>

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
<span data-ttu-id="73d35-508">***参数数组***允许向方法传递数量不定的自变量。</span><span class="sxs-lookup"><span data-stu-id="73d35-508">A ***parameter array*** permits a variable number of arguments to be passed to a method.</span></span> <span data-ttu-id="73d35-509">参数数组使用 `params` 修饰符进行声明。</span><span class="sxs-lookup"><span data-stu-id="73d35-509">A parameter array is declared with the `params` modifier.</span></span> <span data-ttu-id="73d35-510">参数数组只能是方法的最后一个参数，且参数数组的类型必须是一维数组类型。</span><span class="sxs-lookup"><span data-stu-id="73d35-510">Only the last parameter of a method can be a parameter array, and the type of a parameter array must be a single-dimensional array type.</span></span> <span data-ttu-id="73d35-511">`Write`并`WriteLine`方法的`System.Console`类是参数数组用法的典型示例。</span><span class="sxs-lookup"><span data-stu-id="73d35-511">The `Write` and `WriteLine` methods of the `System.Console` class are good examples of parameter array usage.</span></span> <span data-ttu-id="73d35-512">它们的声明方式如下。</span><span class="sxs-lookup"><span data-stu-id="73d35-512">They are declared as follows.</span></span>

```csharp
public class Console
{
    public static void Write(string fmt, params object[] args) {...}
    public static void WriteLine(string fmt, params object[] args) {...}
    ...
}
```
<span data-ttu-id="73d35-513">在使用参数数组的方法中，参数数组的行为与数组类型的常规参数完全相同。</span><span class="sxs-lookup"><span data-stu-id="73d35-513">Within a method that uses a parameter array, the parameter array behaves exactly like a regular parameter of an array type.</span></span> <span data-ttu-id="73d35-514">不过，在调用包含参数数组的方法时，要么可以传递参数数组类型的一个自变量，要么可以传递参数数组的元素类型的任意数量自变量。</span><span class="sxs-lookup"><span data-stu-id="73d35-514">However, in an invocation of a method with a parameter array, it is possible to pass either a single argument of the parameter array type or any number of arguments of the element type of the parameter array.</span></span> <span data-ttu-id="73d35-515">在后一种情况中，数组实例会自动创建，并初始化为包含给定的自变量。</span><span class="sxs-lookup"><span data-stu-id="73d35-515">In the latter case, an array instance is automatically created and initialized with the given arguments.</span></span> <span data-ttu-id="73d35-516">以下示例：</span><span class="sxs-lookup"><span data-stu-id="73d35-516">This example</span></span>

```csharp
Console.WriteLine("x={0} y={1} z={2}", x, y, z);
```
<span data-ttu-id="73d35-517">等同于编写以下代码：</span><span class="sxs-lookup"><span data-stu-id="73d35-517">is equivalent to writing the following.</span></span>

```csharp
string s = "x={0} y={1} z={2}";
object[] args = new object[3];
args[0] = x;
args[1] = y;
args[2] = z;
Console.WriteLine(s, args);
```

#### <a name="method-body-and-local-variables"></a><span data-ttu-id="73d35-518">方法主体和局部变量</span><span class="sxs-lookup"><span data-stu-id="73d35-518">Method body and local variables</span></span>

<span data-ttu-id="73d35-519">方法的正文指定要调用的方法时执行的语句。</span><span class="sxs-lookup"><span data-stu-id="73d35-519">A method's body specifies the statements to execute when the method is invoked.</span></span>

<span data-ttu-id="73d35-520">方法主体可以声明特定于方法调用的变量。</span><span class="sxs-lookup"><span data-stu-id="73d35-520">A method body can declare variables that are specific to the invocation of the method.</span></span> <span data-ttu-id="73d35-521">此类变量称为***局部变量***。</span><span class="sxs-lookup"><span data-stu-id="73d35-521">Such variables are called ***local variables***.</span></span> <span data-ttu-id="73d35-522">局部变量声明指定了类型名称、变量名称以及可能的初始值。</span><span class="sxs-lookup"><span data-stu-id="73d35-522">A local variable declaration specifies a type name, a variable name, and possibly an initial value.</span></span> <span data-ttu-id="73d35-523">下面的示例声明了初始值为零的局部变量 `i` 和无初始值的局部变量 `j`。</span><span class="sxs-lookup"><span data-stu-id="73d35-523">The following example declares a local variable `i` with an initial value of zero and a local variable `j` with no initial value.</span></span>

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
<span data-ttu-id="73d35-524">C# 要求必须先***明确赋值***局部变量，然后才能获取其值。</span><span class="sxs-lookup"><span data-stu-id="73d35-524">C# requires a local variable to be ***definitely assigned*** before its value can be obtained.</span></span> <span data-ttu-id="73d35-525">例如，如果上面的 `i` 声明未包含初始值，那么编译器会在后面使用 `i` 时报告错误，因为在后面使用时 `i` 不会在程序中进行明确赋值。</span><span class="sxs-lookup"><span data-stu-id="73d35-525">For example, if the declaration of the previous `i` did not include an initial value, the compiler would report an error for the subsequent usages of `i` because `i` would not be definitely assigned at those points in the program.</span></span>

<span data-ttu-id="73d35-526">方法可以使用 `return` 语句将控制权返回给调用方。</span><span class="sxs-lookup"><span data-stu-id="73d35-526">A method can use `return` statements to return control to its caller.</span></span> <span data-ttu-id="73d35-527">在返回 `void` 的方法中，`return` 语句无法指定表达式。</span><span class="sxs-lookup"><span data-stu-id="73d35-527">In a method returning `void`, `return` statements cannot specify an expression.</span></span> <span data-ttu-id="73d35-528">在方法中返回非`void`，`return`语句必须包括计算的返回值的表达式。</span><span class="sxs-lookup"><span data-stu-id="73d35-528">In a method returning non-`void`, `return` statements must include an expression that computes the return value.</span></span>

#### <a name="static-and-instance-methods"></a><span data-ttu-id="73d35-529">静态和实例方法</span><span class="sxs-lookup"><span data-stu-id="73d35-529">Static and instance methods</span></span>

<span data-ttu-id="73d35-530">与声明的方法`static`修饰符***静态方法***。</span><span class="sxs-lookup"><span data-stu-id="73d35-530">A method declared with a `static` modifier is a ***static method***.</span></span> <span data-ttu-id="73d35-531">静态方法不对特定的实例起作用，只能直接访问静态成员。</span><span class="sxs-lookup"><span data-stu-id="73d35-531">A static method does not operate on a specific instance and can only directly access static members.</span></span>

<span data-ttu-id="73d35-532">无需声明的方法`static`修饰符***实例方法***。</span><span class="sxs-lookup"><span data-stu-id="73d35-532">A method declared without a `static` modifier is an ***instance method***.</span></span> <span data-ttu-id="73d35-533">实例方法对特定的实例起作用，并能够访问静态和实例成员。</span><span class="sxs-lookup"><span data-stu-id="73d35-533">An instance method operates on a specific instance and can access both static and instance members.</span></span> <span data-ttu-id="73d35-534">其中调用实例方法的实例可以作为 `this` 显式访问。</span><span class="sxs-lookup"><span data-stu-id="73d35-534">The instance on which an instance method was invoked can be explicitly accessed as `this`.</span></span> <span data-ttu-id="73d35-535">在静态方法中引用 `this` 会生成错误。</span><span class="sxs-lookup"><span data-stu-id="73d35-535">It is an error to refer to `this` in a static method.</span></span>

<span data-ttu-id="73d35-536">以下 `Entity` 类包含静态和实例成员。</span><span class="sxs-lookup"><span data-stu-id="73d35-536">The following `Entity` class has both static and instance members.</span></span>

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
<span data-ttu-id="73d35-537">每个 `Entity` 实例均有一个序列号（很可能包含此处未显示的其他一些信息）。</span><span class="sxs-lookup"><span data-stu-id="73d35-537">Each `Entity` instance contains a serial number (and presumably some other information that is not shown here).</span></span> <span data-ttu-id="73d35-538">`Entity` 构造函数（类似于实例方法）将新实例初始化为包含下一个可用的序列号。</span><span class="sxs-lookup"><span data-stu-id="73d35-538">The `Entity` constructor (which is like an instance method) initializes the new instance with the next available serial number.</span></span> <span data-ttu-id="73d35-539">由于构造函数是实例成员，因此可以访问 `serialNo` 实例字段和 `nextSerialNo` 静态字段。</span><span class="sxs-lookup"><span data-stu-id="73d35-539">Because the constructor is an instance member, it is permitted to access both the `serialNo` instance field and the `nextSerialNo` static field.</span></span>

<span data-ttu-id="73d35-540">`GetNextSerialNo` 和 `SetNextSerialNo` 静态方法可以访问 `nextSerialNo` 静态字段，但如果直接访问 `serialNo` 实例字段，则会生成错误。</span><span class="sxs-lookup"><span data-stu-id="73d35-540">The `GetNextSerialNo` and `SetNextSerialNo` static methods can access the `nextSerialNo` static field, but it would be an error for them to directly access the `serialNo` instance field.</span></span>

<span data-ttu-id="73d35-541">下面的示例演示如何使用`Entity`类。</span><span class="sxs-lookup"><span data-stu-id="73d35-541">The following example shows the use of the `Entity` class.</span></span>

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
<span data-ttu-id="73d35-542">请注意，`SetNextSerialNo` 和 `GetNextSerialNo` 静态方法是在类中调用，而 `GetSerialNo` 实例方法则是在类实例中调用。</span><span class="sxs-lookup"><span data-stu-id="73d35-542">Note that the `SetNextSerialNo` and `GetNextSerialNo` static methods are invoked on the class whereas the `GetSerialNo` instance method is invoked on instances of the class.</span></span>

#### <a name="virtual-override-and-abstract-methods"></a><span data-ttu-id="73d35-543">虚方法、重写方法和抽象方法</span><span class="sxs-lookup"><span data-stu-id="73d35-543">Virtual, override, and abstract methods</span></span>

<span data-ttu-id="73d35-544">如果实例方法声明中有 `virtual` 修饰符，可以将实例方法称为“***虚方法***”。</span><span class="sxs-lookup"><span data-stu-id="73d35-544">When an instance method declaration includes a `virtual` modifier, the method is said to be a ***virtual method***.</span></span> <span data-ttu-id="73d35-545">如果未`virtual`修饰符存在，该方法称为***非虚方法***。</span><span class="sxs-lookup"><span data-stu-id="73d35-545">When no `virtual` modifier is present, the method is said to be a ***non-virtual method***.</span></span>

<span data-ttu-id="73d35-546">调用虚方法时，为其调用方法的实例的***运行时类型***决定了要调用的实际方法实现代码。</span><span class="sxs-lookup"><span data-stu-id="73d35-546">When a virtual method is invoked, the ***run-time type*** of the instance for which that invocation takes place determines the actual method implementation to invoke.</span></span> <span data-ttu-id="73d35-547">调用非虚方法时，实例的***编译时类型***是决定性因素。</span><span class="sxs-lookup"><span data-stu-id="73d35-547">In a nonvirtual method invocation, the ***compile-time type*** of the instance is the determining factor.</span></span>

<span data-ttu-id="73d35-548">可以在派生类中***重写***虚方法。</span><span class="sxs-lookup"><span data-stu-id="73d35-548">A virtual method can be ***overridden*** in a derived class.</span></span> <span data-ttu-id="73d35-549">如果实例方法声明包含`override`修饰符，该方法重写继承的虚方法具有相同的签名。</span><span class="sxs-lookup"><span data-stu-id="73d35-549">When an instance method declaration includes an `override` modifier, the method overrides an inherited virtual method with the same signature.</span></span> <span data-ttu-id="73d35-550">但如果虚方法声明中引入新方法，重写方法声明通过提供相应方法的新实现代码，专门针对现有的继承虚方法。</span><span class="sxs-lookup"><span data-stu-id="73d35-550">Whereas a virtual method declaration introduces a new method, an override method declaration specializes an existing inherited virtual method by providing a new implementation of that method.</span></span>

<span data-ttu-id="73d35-551">***抽象***方法是没有实现虚方法。</span><span class="sxs-lookup"><span data-stu-id="73d35-551">An ***abstract*** method is a virtual method with no implementation.</span></span> <span data-ttu-id="73d35-552">一个抽象方法声明具有`abstract`修饰符，但也被声明的类中只允许`abstract`。</span><span class="sxs-lookup"><span data-stu-id="73d35-552">An abstract method is declared with the `abstract` modifier and is permitted only in a class that is also declared `abstract`.</span></span> <span data-ttu-id="73d35-553">必须在所有非抽象派生类中重写抽象方法。</span><span class="sxs-lookup"><span data-stu-id="73d35-553">An abstract method must be overridden in every non-abstract derived class.</span></span>

<span data-ttu-id="73d35-554">下面的示例声明了一个抽象类 `Expression`，用于表示表达式树节点；还声明了三个派生类（`Constant`、`VariableReference` 和 `Operation`），用于实现常量、变量引用和算术运算的表达式树节点。</span><span class="sxs-lookup"><span data-stu-id="73d35-554">The following example declares an abstract class, `Expression`, which represents an expression tree node, and three derived classes, `Constant`, `VariableReference`, and `Operation`, which implement expression tree nodes for constants, variable references, and arithmetic operations.</span></span> <span data-ttu-id="73d35-555">(这是类似，但不要混淆与中的表达式树类型引入[表达式树类型](types.md#expression-tree-types))。</span><span class="sxs-lookup"><span data-stu-id="73d35-555">(This is similar to, but not to be confused with the expression tree types introduced in [Expression tree types](types.md#expression-tree-types)).</span></span>

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
<span data-ttu-id="73d35-556">上面的四个类可用于进行算术表达式建模。</span><span class="sxs-lookup"><span data-stu-id="73d35-556">The previous four classes can be used to model arithmetic expressions.</span></span> <span data-ttu-id="73d35-557">例如，使用这些类的实例，可以按如下方式表示表达式 `x + 3`。</span><span class="sxs-lookup"><span data-stu-id="73d35-557">For example, using instances of these classes, the expression `x + 3` can be represented as follows.</span></span>

```csharp
Expression e = new Operation(
    new VariableReference("x"),
    '+',
    new Constant(3));
```
<span data-ttu-id="73d35-558">调用 `Expression` 实例的 `Evaluate` 方法可以计算给定的表达式并生成 `double` 值。</span><span class="sxs-lookup"><span data-stu-id="73d35-558">The `Evaluate` method of an `Expression` instance is invoked to evaluate the given expression and produce a `double` value.</span></span> <span data-ttu-id="73d35-559">该方法将作为参数`Hashtable`，其中包含变量名称 （作为项键） 和值 （作为项的值）。</span><span class="sxs-lookup"><span data-stu-id="73d35-559">The method takes as an argument a `Hashtable` that contains variable names (as keys of the entries) and values (as values of the entries).</span></span> <span data-ttu-id="73d35-560">`Evaluate`方法是虚拟的抽象方法，这意味着非抽象派生的类必须覆盖它提供一个实际的实现。</span><span class="sxs-lookup"><span data-stu-id="73d35-560">The `Evaluate` method is a virtual abstract method, meaning that non-abstract derived classes must override it to provide an actual implementation.</span></span>

<span data-ttu-id="73d35-561">`Constant` 的 `Evaluate` 实现代码只返回存储的常量。</span><span class="sxs-lookup"><span data-stu-id="73d35-561">A `Constant`'s implementation of `Evaluate` simply returns the stored constant.</span></span> <span data-ttu-id="73d35-562">一个`VariableReference`的实现代码查找哈希表中的变量名称，并返回结果值。</span><span class="sxs-lookup"><span data-stu-id="73d35-562">A `VariableReference`'s implementation looks up the variable name in the hashtable and returns the resulting value.</span></span> <span data-ttu-id="73d35-563">`Operation` 实现代码先计算左右操作数（以递归方式调用其 `Evaluate` 方法），然后执行给定的算术运算。</span><span class="sxs-lookup"><span data-stu-id="73d35-563">An `Operation`'s implementation first evaluates the left and right operands (by recursively invoking their `Evaluate` methods) and then performs the given arithmetic operation.</span></span>

<span data-ttu-id="73d35-564">以下程序使用 `Expression` 类根据不同的 `x` 和 `y` 值计算表达式 `x * (y + 2)`。</span><span class="sxs-lookup"><span data-stu-id="73d35-564">The following program uses the `Expression` classes to evaluate the expression `x * (y + 2)` for different values of `x` and `y`.</span></span>

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

#### <a name="method-overloading"></a><span data-ttu-id="73d35-565">方法重载</span><span class="sxs-lookup"><span data-stu-id="73d35-565">Method overloading</span></span>

<span data-ttu-id="73d35-566">借助方法***重载***，同一类中可以有多个同名的方法，只要这些方法具有唯一签名即可。</span><span class="sxs-lookup"><span data-stu-id="73d35-566">Method ***overloading*** permits multiple methods in the same class to have the same name as long as they have unique signatures.</span></span> <span data-ttu-id="73d35-567">编译如何调用重载的方法时，编译器使用***重载决策***来确定要调用的特定方法。</span><span class="sxs-lookup"><span data-stu-id="73d35-567">When compiling an invocation of an overloaded method, the compiler uses ***overload resolution*** to determine the specific method to invoke.</span></span> <span data-ttu-id="73d35-568">重载决策查找与自变量最匹配的方法；如果找不到最佳匹配项，则会报告错误。</span><span class="sxs-lookup"><span data-stu-id="73d35-568">Overload resolution finds the one method that best matches the arguments or reports an error if no single best match can be found.</span></span> <span data-ttu-id="73d35-569">下面的示例展示了重载决策的实际工作方式。</span><span class="sxs-lookup"><span data-stu-id="73d35-569">The following example shows overload resolution in effect.</span></span> <span data-ttu-id="73d35-570">`Main` 方法中每个调用的注释指明了实际调用的方法。</span><span class="sxs-lookup"><span data-stu-id="73d35-570">The comment for each invocation in the `Main` method shows which method is actually invoked.</span></span>

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
<span data-ttu-id="73d35-571">如示例所示，可以随时将自变量显式转换成确切的参数类型，并/或显式提供类型自变量，从而选择特定的方法。</span><span class="sxs-lookup"><span data-stu-id="73d35-571">As shown by the example, a particular method can always be selected by explicitly casting the arguments to the exact parameter types and/or explicitly supplying type arguments.</span></span>

### <a name="other-function-members"></a><span data-ttu-id="73d35-572">其他函数成员</span><span class="sxs-lookup"><span data-stu-id="73d35-572">Other function members</span></span>

<span data-ttu-id="73d35-573">包含可执行代码的成员统称为类的***函数成员***。</span><span class="sxs-lookup"><span data-stu-id="73d35-573">Members that contain executable code are collectively known as the ***function members*** of a class.</span></span> <span data-ttu-id="73d35-574">上一部分介绍了作为主要函数成员类型的方法。</span><span class="sxs-lookup"><span data-stu-id="73d35-574">The preceding section describes methods, which are the primary kind of function members.</span></span> <span data-ttu-id="73d35-575">本部分介绍其他类型的 C# 支持的函数成员： 构造函数、 属性、 索引器、 事件、 运算符和析构函数。</span><span class="sxs-lookup"><span data-stu-id="73d35-575">This section describes the other kinds of function members supported by C#: constructors, properties, indexers, events, operators, and destructors.</span></span>

<span data-ttu-id="73d35-576">下面的代码演示一个名为的泛型类`List<T>`，它可实现对象的可扩充列表。</span><span class="sxs-lookup"><span data-stu-id="73d35-576">The following code shows a generic class called `List<T>`, which implements a growable list of objects.</span></span> <span data-ttu-id="73d35-577">此类包含最常见类型函数成员的多个示例。</span><span class="sxs-lookup"><span data-stu-id="73d35-577">The class contains several examples of the most common kinds of function members.</span></span>


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

#### <a name="constructors"></a><span data-ttu-id="73d35-578">构造函数</span><span class="sxs-lookup"><span data-stu-id="73d35-578">Constructors</span></span>

<span data-ttu-id="73d35-579">C# 支持实例和静态构造函数。</span><span class="sxs-lookup"><span data-stu-id="73d35-579">C# supports both instance and static constructors.</span></span> <span data-ttu-id="73d35-580">***实例构造函数***是实现初始化类实例所需执行的操作的成员。</span><span class="sxs-lookup"><span data-stu-id="73d35-580">An ***instance constructor*** is a member that implements the actions required to initialize an instance of a class.</span></span> <span data-ttu-id="73d35-581">***静态构造函数***是实现在首次加载类时初始化类本身所需执行的操作的成员。</span><span class="sxs-lookup"><span data-stu-id="73d35-581">A ***static constructor*** is a member that implements the actions required to initialize a class itself when it is first loaded.</span></span>

<span data-ttu-id="73d35-582">构造函数的声明方式与方法一样，都没有返回类型，且与所含类同名。</span><span class="sxs-lookup"><span data-stu-id="73d35-582">A constructor is declared like a method with no return type and the same name as the containing class.</span></span> <span data-ttu-id="73d35-583">如果构造函数声明包含`static`修饰符，它声明了静态构造函数。</span><span class="sxs-lookup"><span data-stu-id="73d35-583">If a constructor declaration includes a `static` modifier, it declares a static constructor.</span></span> <span data-ttu-id="73d35-584">否则，声明的是实例构造函数。</span><span class="sxs-lookup"><span data-stu-id="73d35-584">Otherwise, it declares an instance constructor.</span></span>

<span data-ttu-id="73d35-585">实例构造函数可以进行重载。</span><span class="sxs-lookup"><span data-stu-id="73d35-585">Instance constructors can be overloaded.</span></span> <span data-ttu-id="73d35-586">例如，`List<T>
` 类声明两个实例构造函数：一个没有参数，另一个需要使用 `int` 参数。</span><span class="sxs-lookup"><span data-stu-id="73d35-586">For example, the `List<T>
` class declares two instance constructors, one with no parameters and one that takes an `int` parameter.</span></span> <span data-ttu-id="73d35-587">实例构造函数使用 `new` 运算符进行调用。</span><span class="sxs-lookup"><span data-stu-id="73d35-587">Instance constructors are invoked using the `new` operator.</span></span> <span data-ttu-id="73d35-588">以下语句分配两个`List<string>
`实例使用的构造函数的每个`List`类。</span><span class="sxs-lookup"><span data-stu-id="73d35-588">The following statements allocate two `List<string>
` instances using each of the constructors of the `List` class.</span></span>

```csharp
List<string> list1 = new List<string>();
List<string> list2 = new List<string>(10);
```
<span data-ttu-id="73d35-589">与其他成员不同，实例构造函数不能被继承，且类中只能包含实际已声明的实例构造函数。</span><span class="sxs-lookup"><span data-stu-id="73d35-589">Unlike other members, instance constructors are not inherited, and a class has no instance constructors other than those actually declared in the class.</span></span> <span data-ttu-id="73d35-590">如果没有为类提供实例构造函数，则会自动提供不含参数的空实例构造函数。</span><span class="sxs-lookup"><span data-stu-id="73d35-590">If no instance constructor is supplied for a class, then an empty one with no parameters is automatically provided.</span></span>

#### <a name="properties"></a><span data-ttu-id="73d35-591">属性</span><span class="sxs-lookup"><span data-stu-id="73d35-591">Properties</span></span>

<span data-ttu-id="73d35-592">***属性***是字段的自然扩展。</span><span class="sxs-lookup"><span data-stu-id="73d35-592">***Properties*** are a natural extension of fields.</span></span> <span data-ttu-id="73d35-593">两者都是包含关联类型的已命名成员，用于访问字段和属性的语法也是一样的。</span><span class="sxs-lookup"><span data-stu-id="73d35-593">Both are named members with associated types, and the syntax for accessing fields and properties is the same.</span></span> <span data-ttu-id="73d35-594">不过，与字段不同的是，属性不指明存储位置。</span><span class="sxs-lookup"><span data-stu-id="73d35-594">However, unlike fields, properties do not denote storage locations.</span></span> <span data-ttu-id="73d35-595">相反，属性包含***访问器***，用于指定在读取或写入属性值时要执行的语句。</span><span class="sxs-lookup"><span data-stu-id="73d35-595">Instead, properties have ***accessors*** that specify the statements to be executed when their values are read or written.</span></span>

<span data-ttu-id="73d35-596">某个属性声明字段类似，只不过在声明结尾`get`访问器和/或`set`访问器编写分隔符之间`{`和`}`而不是以分号结尾。</span><span class="sxs-lookup"><span data-stu-id="73d35-596">A property is declared like a field, except that the declaration ends with a `get` accessor and/or a `set` accessor written between the delimiters `{` and `}` instead of ending in a semicolon.</span></span> <span data-ttu-id="73d35-597">同时具有一个属性`get`访问器和一个`set`访问器已***读-写属性***，仅具有一个属性`get`访问器是***只读属性***，和一个仅具有的属性`set`访问器已***只写属性***。</span><span class="sxs-lookup"><span data-stu-id="73d35-597">A property that has both a `get` accessor and a `set` accessor is a ***read-write property***, a property that has only a `get` accessor is a ***read-only property***, and a property that has only a `set` accessor is a ***write-only property***.</span></span>

<span data-ttu-id="73d35-598">一个`get`访问器对应于具有返回值的属性类型的无参数方法。</span><span class="sxs-lookup"><span data-stu-id="73d35-598">A `get` accessor corresponds to a parameterless method with a return value of the property type.</span></span> <span data-ttu-id="73d35-599">当在表达式中，引用属性除了作为赋值目标`get`属性访问器调用以计算属性的值。</span><span class="sxs-lookup"><span data-stu-id="73d35-599">Except as the target of an assignment, when a property is referenced in an expression, the `get` accessor of the property is invoked to compute the value of the property.</span></span>

<span data-ttu-id="73d35-600">一个`set`访问器对应于一种方法具有一个名为的单个参数`value`且没有返回类型。</span><span class="sxs-lookup"><span data-stu-id="73d35-600">A `set` accessor corresponds to a method with a single parameter named `value` and no return type.</span></span> <span data-ttu-id="73d35-601">为作为赋值目标或的操作数时引用属性`++`或`--`，则`set`用提供的新值的参数调用访问器。</span><span class="sxs-lookup"><span data-stu-id="73d35-601">When a property is referenced as the target of an assignment or as the operand of `++` or `--`, the `set` accessor is invoked with an argument that provides the new value.</span></span>

<span data-ttu-id="73d35-602">`List<T>
`类中声明两个属性`Count`和`Capacity`，分别是只读和读写。</span><span class="sxs-lookup"><span data-stu-id="73d35-602">The `List<T>
` class declares two properties, `Count` and `Capacity`, which are read-only and read-write, respectively.</span></span> <span data-ttu-id="73d35-603">下面的示例展示了如何使用这些属性。</span><span class="sxs-lookup"><span data-stu-id="73d35-603">The following is an example of use of these properties.</span></span>

```csharp
List<string> names = new List<string>();
names.Capacity = 100;            // Invokes set accessor
int i = names.Count;             // Invokes get accessor
int j = names.Capacity;          // Invokes get accessor
```
<span data-ttu-id="73d35-604">类似于字段和方法，C# 支持实例属性和静态属性。</span><span class="sxs-lookup"><span data-stu-id="73d35-604">Similar to fields and methods, C# supports both instance properties and static properties.</span></span> <span data-ttu-id="73d35-605">静态属性的声明与`static`没有它声明修饰符和实例属性。</span><span class="sxs-lookup"><span data-stu-id="73d35-605">Static properties are declared with the `static` modifier, and instance properties are declared without it.</span></span>

<span data-ttu-id="73d35-606">属性的访问器可以是虚的。</span><span class="sxs-lookup"><span data-stu-id="73d35-606">The accessor(s) of a property can be virtual.</span></span> <span data-ttu-id="73d35-607">如果属性声明包含 `virtual`、`abstract` 或 `override` 修饰符，则适用于属性的访问器。</span><span class="sxs-lookup"><span data-stu-id="73d35-607">When a property declaration includes a `virtual`, `abstract`, or `override` modifier, it applies to the accessor(s) of the property.</span></span>

#### <a name="indexers"></a><span data-ttu-id="73d35-608">索引器</span><span class="sxs-lookup"><span data-stu-id="73d35-608">Indexers</span></span>

<span data-ttu-id="73d35-609">借助***索引器***成员，可以将对象编入索引（像处理数组一样）。</span><span class="sxs-lookup"><span data-stu-id="73d35-609">An ***indexer*** is a member that enables objects to be indexed in the same way as an array.</span></span> <span data-ttu-id="73d35-610">索引器的声明与属性类似，不同的成员的名称是`this`分隔符之间写入参数列表后跟`[`和`]`。</span><span class="sxs-lookup"><span data-stu-id="73d35-610">An indexer is declared like a property except that the name of the member is `this` followed by a parameter list written between the delimiters `[` and `]`.</span></span> <span data-ttu-id="73d35-611">这些参数在索引器的访问器中可用。</span><span class="sxs-lookup"><span data-stu-id="73d35-611">The parameters are available in the accessor(s) of the indexer.</span></span> <span data-ttu-id="73d35-612">类似于属性，索引器分为读写、只读和只写索引器，且索引器的访问器可以是虚的。</span><span class="sxs-lookup"><span data-stu-id="73d35-612">Similar to properties, indexers can be read-write, read-only, and write-only, and the accessor(s) of an indexer can be virtual.</span></span>

<span data-ttu-id="73d35-613">`List` 类声明一个需要使用 `int` 参数的读写索引器。</span><span class="sxs-lookup"><span data-stu-id="73d35-613">The `List` class declares a single read-write indexer that takes an `int` parameter.</span></span> <span data-ttu-id="73d35-614">借助索引器，可以使用 `int` 值将 `List` 实例编入索引。</span><span class="sxs-lookup"><span data-stu-id="73d35-614">The indexer makes it possible to index `List` instances with `int` values.</span></span> <span data-ttu-id="73d35-615">例如</span><span class="sxs-lookup"><span data-stu-id="73d35-615">For example</span></span>

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
<span data-ttu-id="73d35-616">索引器可以进行重载。也就是说，类可以声明多个索引器，只要其参数的数量或类型不同即可。</span><span class="sxs-lookup"><span data-stu-id="73d35-616">Indexers can be overloaded, meaning that a class can declare multiple indexers as long as the number or types of their parameters differ.</span></span>

#### <a name="events"></a><span data-ttu-id="73d35-617">事件</span><span class="sxs-lookup"><span data-stu-id="73d35-617">Events</span></span>

<span data-ttu-id="73d35-618">借助***事件***成员，类或对象可以提供通知。</span><span class="sxs-lookup"><span data-stu-id="73d35-618">An ***event*** is a member that enables a class or object to provide notifications.</span></span> <span data-ttu-id="73d35-619">事件的声明与字段类似，不同的声明包含`event`关键字和类型必须是委托类型。</span><span class="sxs-lookup"><span data-stu-id="73d35-619">An event is declared like a field except that the declaration includes an `event` keyword and the type must be a delegate type.</span></span>

<span data-ttu-id="73d35-620">在声明事件成员的类中，事件的行为与委托类型的字段完全相同（前提是事件不是抽象的，且不声明访问器）。</span><span class="sxs-lookup"><span data-stu-id="73d35-620">Within a class that declares an event member, the event behaves just like a field of a delegate type (provided the event is not abstract and does not declare accessors).</span></span> <span data-ttu-id="73d35-621">字段存储对委托的引用，委托表示已添加到事件的事件处理程序。</span><span class="sxs-lookup"><span data-stu-id="73d35-621">The field stores a reference to a delegate that represents the event handlers that have been added to the event.</span></span> <span data-ttu-id="73d35-622">如果没有事件处理程序，该字段是`null`。</span><span class="sxs-lookup"><span data-stu-id="73d35-622">If no event handles are present, the field is `null`.</span></span>

<span data-ttu-id="73d35-623">`List<T>
` 类声明一个 `Changed` 事件成员，指明已向列表添加了新项。</span><span class="sxs-lookup"><span data-stu-id="73d35-623">The `List<T>
` class declares a single event member called `Changed`, which indicates that a new item has been added to the list.</span></span> <span data-ttu-id="73d35-624">`Changed`引发事件`OnChanged`虚拟方法，以便先检查是否`null`（这意味着没有处理程序是否存在）。</span><span class="sxs-lookup"><span data-stu-id="73d35-624">The `Changed` event is raised by the `OnChanged` virtual method, which first checks whether the event is `null` (meaning that no handlers are present).</span></span> <span data-ttu-id="73d35-625">引发事件的概念恰恰等同于调用由事件表示的委托，因此，没有用于引发事件的特殊语言构造。</span><span class="sxs-lookup"><span data-stu-id="73d35-625">The notion of raising an event is precisely equivalent to invoking the delegate represented by the event—thus, there are no special language constructs for raising events.</span></span>

<span data-ttu-id="73d35-626">客户端通过***事件处理程序***响应事件。</span><span class="sxs-lookup"><span data-stu-id="73d35-626">Clients react to events through ***event handlers***.</span></span> <span data-ttu-id="73d35-627">使用 `+=` 和 `-=` 运算符分别可以附加和删除事件处理程序。</span><span class="sxs-lookup"><span data-stu-id="73d35-627">Event handlers are attached using the `+=` operator and removed using the `-=` operator.</span></span> <span data-ttu-id="73d35-628">下面的示例展示了如何向 `List<string>
` 的 `Changed` 事件附加事件处理程序。</span><span class="sxs-lookup"><span data-stu-id="73d35-628">The following example attaches an event handler to the `Changed` event of a `List<string>
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
<span data-ttu-id="73d35-629">对于需要控制事件的基础存储的高级方案，事件声明可以显式提供 `add` 和 `remove` 访问器，这在某种程度上与属性的 `set` 访问器类似。</span><span class="sxs-lookup"><span data-stu-id="73d35-629">For advanced scenarios where control of the underlying storage of an event is desired, an event declaration can explicitly provide `add` and `remove` accessors, which are somewhat similar to the `set` accessor of a property.</span></span>

#### <a name="operators"></a><span data-ttu-id="73d35-630">运算符</span><span class="sxs-lookup"><span data-stu-id="73d35-630">Operators</span></span>

<span data-ttu-id="73d35-631">***运算符***是定义向类实例应用特定表达式运算符的含义的成员。</span><span class="sxs-lookup"><span data-stu-id="73d35-631">An ***operator*** is a member that defines the meaning of applying a particular expression operator to instances of a class.</span></span> <span data-ttu-id="73d35-632">可以定义三种类型的运算符：一元运算符、二元运算符和转换运算符。</span><span class="sxs-lookup"><span data-stu-id="73d35-632">Three kinds of operators can be defined: unary operators, binary operators, and conversion operators.</span></span> <span data-ttu-id="73d35-633">所有运算符都必须声明为 `public` 和 `static`。</span><span class="sxs-lookup"><span data-stu-id="73d35-633">All operators must be declared as `public` and `static`.</span></span>

<span data-ttu-id="73d35-634">`List<T>
` 类声明两个运算符（`operator==` 和 `operator!=`），因此定义了向 `List` 实例应用这些运算符的表达式的新含义。</span><span class="sxs-lookup"><span data-stu-id="73d35-634">The `List<T>
` class declares two operators, `operator==` and `operator!=`, and thus gives new meaning to expressions that apply those operators to `List` instances.</span></span> <span data-ttu-id="73d35-635">具体而言，这些运算符定义两个相等`List<T>
`实例作为比较每个包含的对象使用其`Equals`方法。</span><span class="sxs-lookup"><span data-stu-id="73d35-635">Specifically, the operators define equality of two `List<T>
` instances as comparing each of the contained objects using their `Equals` methods.</span></span> <span data-ttu-id="73d35-636">下面的示例展示了如何使用 `==` 运算符比较两个 `List<int>
` 实例。</span><span class="sxs-lookup"><span data-stu-id="73d35-636">The following example uses the `==` operator to compare two `List<int>
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

<span data-ttu-id="73d35-637">第一个 `Console.WriteLine` 输出 `True`，因为两个列表包含的对象不仅数量相同，而且值和顺序也相同。</span><span class="sxs-lookup"><span data-stu-id="73d35-637">The first `Console.WriteLine` outputs `True` because the two lists contain the same number of objects with the same values in the same order.</span></span> <span data-ttu-id="73d35-638">如果 `List<T>
` 未定义 `operator==`，那么第一个 `Console.WriteLine` 会输出 `False`，因为 `a` 和 `b` 引用不同的 `List<int>
` 实例。</span><span class="sxs-lookup"><span data-stu-id="73d35-638">Had `List<T>
` not defined `operator==`, the first `Console.WriteLine` would have output `False` because `a` and `b` reference different `List<int>
` instances.</span></span>

#### <a name="destructors"></a><span data-ttu-id="73d35-639">析构函数</span><span class="sxs-lookup"><span data-stu-id="73d35-639">Destructors</span></span>

<span data-ttu-id="73d35-640">一个***析构函数***是实现析构类的实例所必需的操作的成员。</span><span class="sxs-lookup"><span data-stu-id="73d35-640">A ***destructor*** is a member that implements the actions required to destruct an instance of a class.</span></span> <span data-ttu-id="73d35-641">析构函数不能有参数，它们不能具有可访问性修饰符不能显式调用。</span><span class="sxs-lookup"><span data-stu-id="73d35-641">Destructors cannot have parameters, they cannot have accessibility modifiers, and they cannot be invoked explicitly.</span></span> <span data-ttu-id="73d35-642">在垃圾回收期间自动调用实例的析构函数。</span><span class="sxs-lookup"><span data-stu-id="73d35-642">The destructor for an instance is invoked automatically during garbage collection.</span></span>

<span data-ttu-id="73d35-643">垃圾回收器很大自由度中确定何时收集对象和运行析构函数。</span><span class="sxs-lookup"><span data-stu-id="73d35-643">The garbage collector is allowed wide latitude in deciding when to collect objects and run destructors.</span></span> <span data-ttu-id="73d35-644">具体而言，是不确定性的析构函数调用的计时和析构函数可能在任何线程上执行。</span><span class="sxs-lookup"><span data-stu-id="73d35-644">Specifically, the timing of destructor invocations is not deterministic, and destructors may be executed on any thread.</span></span> <span data-ttu-id="73d35-645">有关这些和其他原因，类应仅当没有其他解决方案都可行时实现析构函数。</span><span class="sxs-lookup"><span data-stu-id="73d35-645">For these and other reasons, classes should implement destructors only when no other solutions are feasible.</span></span>

<span data-ttu-id="73d35-646">处理对象析构的更好方法是使用 `using` 语句。</span><span class="sxs-lookup"><span data-stu-id="73d35-646">The `using` statement provides a better approach to object destruction.</span></span>

## <a name="structs"></a><span data-ttu-id="73d35-647">结构</span><span class="sxs-lookup"><span data-stu-id="73d35-647">Structs</span></span>

<span data-ttu-id="73d35-648">***结构***是可以包含数据成员和函数成员的数据结构，这一点与类一样；与类不同的是，结构是值类型，无需进行堆分配。</span><span class="sxs-lookup"><span data-stu-id="73d35-648">Like classes, ***structs*** are data structures that can contain data members and function members, but unlike classes, structs are value types and do not require heap allocation.</span></span> <span data-ttu-id="73d35-649">结构类型的变量直接存储结构数据，而类类型的变量存储对动态分配的对象的引用。</span><span class="sxs-lookup"><span data-stu-id="73d35-649">A variable of a struct type directly stores the data of the struct, whereas a variable of a class type stores a reference to a dynamically allocated object.</span></span> <span data-ttu-id="73d35-650">结构类型不支持用户指定的继承，并且所有结构类型均隐式继承自类型 `object`。</span><span class="sxs-lookup"><span data-stu-id="73d35-650">Struct types do not support user-specified inheritance, and all struct types implicitly inherit from type `object`.</span></span>

<span data-ttu-id="73d35-651">结构对包含值语义的小型数据结构特别有用。</span><span class="sxs-lookup"><span data-stu-id="73d35-651">Structs are particularly useful for small data structures that have value semantics.</span></span> <span data-ttu-id="73d35-652">复数、坐标系中的点或字典中的键值对都是结构的典型示例。</span><span class="sxs-lookup"><span data-stu-id="73d35-652">Complex numbers, points in a coordinate system, or key-value pairs in a dictionary are all good examples of structs.</span></span> <span data-ttu-id="73d35-653">对小型数据结构使用结构（而不是类）在应用程序执行的内存分配次数上存在巨大差异。</span><span class="sxs-lookup"><span data-stu-id="73d35-653">The use of structs rather than classes for small data structures can make a large difference in the number of memory allocations an application performs.</span></span> <span data-ttu-id="73d35-654">例如，以下程序创建并初始化包含 100 个点的数组。</span><span class="sxs-lookup"><span data-stu-id="73d35-654">For example, the following program creates and initializes an array of 100 points.</span></span> <span data-ttu-id="73d35-655">通过将 `Point` 实现为类，可单独实例化 101 个对象，一个对象用于数组，其他所有对象分别用于 100 个元素。</span><span class="sxs-lookup"><span data-stu-id="73d35-655">With `Point` implemented as a class, 101 separate objects are instantiated—one for the array and one each for the 100 elements.</span></span>

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
<span data-ttu-id="73d35-656">一种替代方法是使`Point`结构。</span><span class="sxs-lookup"><span data-stu-id="73d35-656">An alternative is to make `Point` a struct.</span></span>

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
<span data-ttu-id="73d35-657">现在，仅实例化一个对象（即用于数组的对象），`Point` 实例存储内嵌在数组中。</span><span class="sxs-lookup"><span data-stu-id="73d35-657">Now, only one object is instantiated—the one for the array—and the `Point` instances are stored in-line in the array.</span></span>

<span data-ttu-id="73d35-658">结构构造函数使用 `new` 运算符进行调用，但这不并表示要分配内存。</span><span class="sxs-lookup"><span data-stu-id="73d35-658">Struct constructors are invoked with the `new` operator, but that does not imply that memory is being allocated.</span></span> <span data-ttu-id="73d35-659">结构构造函数只返回结构值本身（通常在堆栈的临时位置中），并在必要时复制此值，而非动态分配对象并返回对此对象的引用。</span><span class="sxs-lookup"><span data-stu-id="73d35-659">Instead of dynamically allocating an object and returning a reference to it, a struct constructor simply returns the struct value itself (typically in a temporary location on the stack), and this value is then copied as necessary.</span></span>

<span data-ttu-id="73d35-660">借助类，两个变量可以引用同一对象；因此，对一个变量执行的运算可能会影响另一个变量引用的对象。</span><span class="sxs-lookup"><span data-stu-id="73d35-660">With classes, it is possible for two variables to reference the same object and thus possible for operations on one variable to affect the object referenced by the other variable.</span></span> <span data-ttu-id="73d35-661">借助结构，每个变量都有自己的数据副本；因此，对一个变量执行的运算不会影响另一个变量。</span><span class="sxs-lookup"><span data-stu-id="73d35-661">With structs, the variables each have their own copy of the data, and it is not possible for operations on one to affect the other.</span></span> <span data-ttu-id="73d35-662">例如，下面的代码段生成的输出取决于是否`Point`是类还是结构。</span><span class="sxs-lookup"><span data-stu-id="73d35-662">For example, the output produced by the following code fragment depends on whether `Point` is a class or a struct.</span></span>

```csharp
Point a = new Point(10, 10);
Point b = a;
a.x = 20;
Console.WriteLine(b.x);
```
<span data-ttu-id="73d35-663">如果`Point`是一个类，则输出`20`因为`a`和`b`引用相同的对象。</span><span class="sxs-lookup"><span data-stu-id="73d35-663">If `Point` is a class, the output is `20` because `a` and `b` reference the same object.</span></span> <span data-ttu-id="73d35-664">如果`Point`是一种结构，输出是`10`因为分配`a`到`b`会创建一份值，而此副本不受后续分配到`a.x`。</span><span class="sxs-lookup"><span data-stu-id="73d35-664">If `Point` is a struct, the output is `10` because the assignment of `a` to `b` creates a copy of the value, and this copy is unaffected by the subsequent assignment to `a.x`.</span></span>

<span data-ttu-id="73d35-665">以上示例突出显示了结构的两个限制。</span><span class="sxs-lookup"><span data-stu-id="73d35-665">The previous example highlights two of the limitations of structs.</span></span> <span data-ttu-id="73d35-666">首先，复制整个结构通常比复制对象引用效率更低，因此通过结构进行的赋值和值参数传递可能比通过引用类型成本更高。</span><span class="sxs-lookup"><span data-stu-id="73d35-666">First, copying an entire struct is typically less efficient than copying an object reference, so assignment and value parameter passing can be more expensive with structs than with reference types.</span></span> <span data-ttu-id="73d35-667">其次，除 `ref` 和 `out` 参数以外，无法创建对结构的引用，这就表示在很多应用场景中都不能使用结构。</span><span class="sxs-lookup"><span data-stu-id="73d35-667">Second, except for `ref` and `out` parameters, it is not possible to create references to structs, which rules out their usage in a number of situations.</span></span>

## <a name="arrays"></a><span data-ttu-id="73d35-668">数组</span><span class="sxs-lookup"><span data-stu-id="73d35-668">Arrays</span></span>

<span data-ttu-id="73d35-669">***数组***是一种数据结构，其中包含许多通过计算索引访问的变量。</span><span class="sxs-lookup"><span data-stu-id="73d35-669">An ***array*** is a data structure that contains a number of variables that are accessed through computed indices.</span></span> <span data-ttu-id="73d35-670">数组中的变量（亦称为数组的***元素***）均为同一种类型，我们将这种类型称为数组的***元素类型***。</span><span class="sxs-lookup"><span data-stu-id="73d35-670">The variables contained in an array, also called the ***elements*** of the array, are all of the same type, and this type is called the ***element type*** of the array.</span></span>

<span data-ttu-id="73d35-671">数组类型是引用类型，声明数组变量只是为引用数组实例预留空间。</span><span class="sxs-lookup"><span data-stu-id="73d35-671">Array types are reference types, and the declaration of an array variable simply sets aside space for a reference to an array instance.</span></span> <span data-ttu-id="73d35-672">在运行时使用动态创建实际数组实例`new`运算符。</span><span class="sxs-lookup"><span data-stu-id="73d35-672">Actual array instances are created dynamically at run-time using the `new` operator.</span></span> <span data-ttu-id="73d35-673">`new`操作指定***长度***新数组实例，然后实例的生存期内固定。</span><span class="sxs-lookup"><span data-stu-id="73d35-673">The `new` operation specifies the ***length*** of the new array instance, which is then fixed for the lifetime of the instance.</span></span> <span data-ttu-id="73d35-674">数组元素的索引介于 `0` 到 `Length - 1` 之间。</span><span class="sxs-lookup"><span data-stu-id="73d35-674">The indices of the elements of an array range from `0` to `Length - 1`.</span></span> <span data-ttu-id="73d35-675">`new` 运算符自动将数组元素初始化为其默认值（例如，所有数值类型的默认值为 0，所有引用类型的默认值为 `null`）。</span><span class="sxs-lookup"><span data-stu-id="73d35-675">The `new` operator automatically initializes the elements of an array to their default value, which, for example, is zero for all numeric types and `null` for all reference types.</span></span>

<span data-ttu-id="73d35-676">以下示例创建 `int` 元素数组，初始化此数组，然后打印输出此数组的内容。</span><span class="sxs-lookup"><span data-stu-id="73d35-676">The following example creates an array of `int` elements, initializes the array, and prints out the contents of the array.</span></span>

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
<span data-ttu-id="73d35-677">上面的示例创建***一维数组***，并对其执行运算。</span><span class="sxs-lookup"><span data-stu-id="73d35-677">This example creates and operates on a ***single-dimensional array***.</span></span> <span data-ttu-id="73d35-678">C# 还支持***多维数组***。</span><span class="sxs-lookup"><span data-stu-id="73d35-678">C# also supports ***multi-dimensional arrays***.</span></span> <span data-ttu-id="73d35-679">数组类型的维数（亦称为数组类型的***秩***）是 1 与数组类型方括号内的逗号数量相加的结果。</span><span class="sxs-lookup"><span data-stu-id="73d35-679">The number of dimensions of an array type, also known as the ***rank*** of the array type, is one plus the number of commas written between the square brackets of the array type.</span></span> <span data-ttu-id="73d35-680">以下示例分配一个一维、 二维和三维数组。</span><span class="sxs-lookup"><span data-stu-id="73d35-680">The following example allocates a one-dimensional, a two-dimensional, and a three-dimensional array.</span></span>

```csharp
int[] a1 = new int[10];
int[,] a2 = new int[10, 5];
int[,,] a3 = new int[10, 5, 2];
```
<span data-ttu-id="73d35-681">`a1` 数组包含 10 个元素，`a2` 数组包含 50 个元素 (10 × 5)，`a3` 数组包含 100 个元素 (10 × 5 × 2)。</span><span class="sxs-lookup"><span data-stu-id="73d35-681">The `a1` array contains 10 elements, the `a2` array contains 50 (10 × 5) elements, and the `a3` array contains 100 (10 × 5 × 2) elements.</span></span>

<span data-ttu-id="73d35-682">数组的元素类型可以是任意类型（包括数组类型）。</span><span class="sxs-lookup"><span data-stu-id="73d35-682">The element type of an array can be any type, including an array type.</span></span> <span data-ttu-id="73d35-683">包含数组类型元素的数组有时称为***交错数组***，因为元素数组的长度不必全都一样。</span><span class="sxs-lookup"><span data-stu-id="73d35-683">An array with elements of an array type is sometimes called a ***jagged array*** because the lengths of the element arrays do not all have to be the same.</span></span> <span data-ttu-id="73d35-684">以下示例分配由 `int` 数组构成的数组：</span><span class="sxs-lookup"><span data-stu-id="73d35-684">The following example allocates an array of arrays of `int`:</span></span>

```csharp
int[][] a = new int[3][];
a[0] = new int[10];
a[1] = new int[5];
a[2] = new int[20];
```
<span data-ttu-id="73d35-685">第一行创建包含三个元素的数组，每个元素都是 `int[]` 类型，并且初始值均为 `null`。</span><span class="sxs-lookup"><span data-stu-id="73d35-685">The first line creates an array with three elements, each of type `int[]` and each with an initial value of `null`.</span></span> <span data-ttu-id="73d35-686">后面的代码行将这三个元素初始化为引用长度不同的各个数组实例。</span><span class="sxs-lookup"><span data-stu-id="73d35-686">The subsequent lines then initialize the three elements with references to individual array instances of varying lengths.</span></span>

<span data-ttu-id="73d35-687">`new`运算符，可以使用指定的数组元素的初始值***数组初始值设定项***，这是一系列在分隔符编写的表达式`{`和`}`。</span><span class="sxs-lookup"><span data-stu-id="73d35-687">The `new` operator permits the initial values of the array elements to be specified using an ***array initializer***, which is a list of expressions written between the delimiters `{` and `}`.</span></span> <span data-ttu-id="73d35-688">以下示例分配 `int[]`，并将其初始化为包含三个元素。</span><span class="sxs-lookup"><span data-stu-id="73d35-688">The following example allocates and initializes an `int[]` with three elements.</span></span>

```csharp
int[] a = new int[] {1, 2, 3};
```
<span data-ttu-id="73d35-689">请注意从内的表达式数量推断出数组的长度`{`和`}`。</span><span class="sxs-lookup"><span data-stu-id="73d35-689">Note that the length of the array is inferred from the number of expressions between `{` and `}`.</span></span> <span data-ttu-id="73d35-690">局部变量和字段声明可以进一步缩短，这样就不用重新声明数组类型了。</span><span class="sxs-lookup"><span data-stu-id="73d35-690">Local variable and field declarations can be shortened further such that the array type does not have to be restated.</span></span>

```csharp
int[] a = {1, 2, 3};
```
<span data-ttu-id="73d35-691">以上两个示例等同于以下示例：</span><span class="sxs-lookup"><span data-stu-id="73d35-691">Both of the previous examples are equivalent to the following:</span></span>

```csharp
int[] t = new int[3];
t[0] = 1;
t[1] = 2;
t[2] = 3;
int[] a = t;
```
## <a name="interfaces"></a><span data-ttu-id="73d35-692">接口</span><span class="sxs-lookup"><span data-stu-id="73d35-692">Interfaces</span></span>

<span data-ttu-id="73d35-693">***接口***定义了可由类和结构实现的协定。</span><span class="sxs-lookup"><span data-stu-id="73d35-693">An ***interface*** defines a contract that can be implemented by classes and structs.</span></span> <span data-ttu-id="73d35-694">接口可以包含方法、属性、事件和索引器。</span><span class="sxs-lookup"><span data-stu-id="73d35-694">An interface can contain methods, properties, events, and indexers.</span></span> <span data-ttu-id="73d35-695">接口不提供所定义的成员的实现代码，仅指定必须由实现接口的类或结构提供的成员。</span><span class="sxs-lookup"><span data-stu-id="73d35-695">An interface does not provide implementations of the members it defines—it merely specifies the members that must be supplied by classes or structs that implement the interface.</span></span>

<span data-ttu-id="73d35-696">接口可以采用***多重继承***。</span><span class="sxs-lookup"><span data-stu-id="73d35-696">Interfaces may employ ***multiple inheritance***.</span></span> <span data-ttu-id="73d35-697">在以下示例中，接口 `IComboBox` 同时继承自 `ITextBox` 和 `IListBox`。</span><span class="sxs-lookup"><span data-stu-id="73d35-697">In the following example, the interface `IComboBox` inherits from both `ITextBox` and `IListBox`.</span></span>

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
<span data-ttu-id="73d35-698">类和结构可以实现多个接口。</span><span class="sxs-lookup"><span data-stu-id="73d35-698">Classes and structs can implement multiple interfaces.</span></span> <span data-ttu-id="73d35-699">在以下示例中，类 `EditBox` 同时实现 `IControl` 和 `IDataBound`。</span><span class="sxs-lookup"><span data-stu-id="73d35-699">In the following example, the class `EditBox` implements both `IControl` and `IDataBound`.</span></span>

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
<span data-ttu-id="73d35-700">当类或结构实现特定接口时，此类或结构的实例可以隐式转换成相应的接口类型。</span><span class="sxs-lookup"><span data-stu-id="73d35-700">When a class or struct implements a particular interface, instances of that class or struct can be implicitly converted to that interface type.</span></span> <span data-ttu-id="73d35-701">例如</span><span class="sxs-lookup"><span data-stu-id="73d35-701">For example</span></span>

```csharp
EditBox editBox = new EditBox();
IControl control = editBox;
IDataBound dataBound = editBox;
```
<span data-ttu-id="73d35-702">如果已知实例不是静态地实现特定接口，可以使用动态类型显式转换功能。</span><span class="sxs-lookup"><span data-stu-id="73d35-702">In cases where an instance is not statically known to implement a particular interface, dynamic type casts can be used.</span></span> <span data-ttu-id="73d35-703">例如，以下语句使用动态类型强制转换获取对象的`IControl`和`IDataBound`接口实现代码。</span><span class="sxs-lookup"><span data-stu-id="73d35-703">For example, the following statements use dynamic type casts to obtain an object's `IControl` and `IDataBound` interface implementations.</span></span> <span data-ttu-id="73d35-704">因为该对象的实际类型是`EditBox`，显式转换会成功。</span><span class="sxs-lookup"><span data-stu-id="73d35-704">Because the actual type of the object is `EditBox`, the casts succeed.</span></span>

```csharp
object obj = new EditBox();
IControl control = (IControl)obj;
IDataBound dataBound = (IDataBound)obj;
```
<span data-ttu-id="73d35-705">在前面`EditBox`类，`Paint`方法从`IControl`接口并`Bind`方法从`IDataBound`使用实现接口`public`成员。</span><span class="sxs-lookup"><span data-stu-id="73d35-705">In the previous `EditBox` class, the `Paint` method from the `IControl` interface and the `Bind` method from the `IDataBound` interface are implemented using `public` members.</span></span> <span data-ttu-id="73d35-706">C# 还支持***显式接口成员实现代码***，使用这类或结构可避免创建成员`public`。</span><span class="sxs-lookup"><span data-stu-id="73d35-706">C# also supports ***explicit interface member implementations***, using which the class or struct can avoid making the members `public`.</span></span> <span data-ttu-id="73d35-707">显式接口成员实现代码是使用完全限定的接口成员名称进行编写。</span><span class="sxs-lookup"><span data-stu-id="73d35-707">An explicit interface member implementation is written using the fully qualified interface member name.</span></span> <span data-ttu-id="73d35-708">例如，`EditBox` 类可以使用显式接口成员实现代码来实现 `IControl.Paint` 和 `IDataBound.Bind` 方法，如下所示。</span><span class="sxs-lookup"><span data-stu-id="73d35-708">For example, the `EditBox` class could implement the `IControl.Paint` and `IDataBound.Bind` methods using explicit interface member implementations as follows.</span></span>

```csharp
public class EditBox: IControl, IDataBound
{
    void IControl.Paint() {...}
    void IDataBound.Bind(Binder b) {...}
}
```
<span data-ttu-id="73d35-709">显式接口成员只能通过接口类型进行访问。</span><span class="sxs-lookup"><span data-stu-id="73d35-709">Explicit interface members can only be accessed via the interface type.</span></span> <span data-ttu-id="73d35-710">例如，实现`IControl.Paint`由上一个提供`EditBox`类只能调用通过第一个转换`EditBox`引用添加到`IControl`接口类型。</span><span class="sxs-lookup"><span data-stu-id="73d35-710">For example, the implementation of `IControl.Paint` provided by the previous `EditBox` class can only be invoked by first converting the `EditBox` reference to the `IControl` interface type.</span></span>

```csharp
EditBox editBox = new EditBox();
editBox.Paint();                        // Error, no such method
IControl control = editBox;
control.Paint();                        // Ok
```

## <a name="enums"></a><span data-ttu-id="73d35-711">枚举</span><span class="sxs-lookup"><span data-stu-id="73d35-711">Enums</span></span>

<span data-ttu-id="73d35-712">***枚举类型***是包含一组已命名常量的独特值类型。</span><span class="sxs-lookup"><span data-stu-id="73d35-712">An ***enum type*** is a distinct value type with a set of named constants.</span></span> <span data-ttu-id="73d35-713">以下示例声明并使用名为枚举类型`Color`包含三个常量值`Red`， `Green`，和`Blue`。</span><span class="sxs-lookup"><span data-stu-id="73d35-713">The following example declares and uses an enum type named `Color` with three constant values, `Red`, `Green`, and `Blue`.</span></span>

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
<span data-ttu-id="73d35-714">每个枚举类型具有对应的整型类型称为***基础类型***的枚举类型。</span><span class="sxs-lookup"><span data-stu-id="73d35-714">Each enum type has a corresponding integral type called the ***underlying type*** of the enum type.</span></span> <span data-ttu-id="73d35-715">未显式声明基础类型的枚举类型有一个基础类型的`int`。</span><span class="sxs-lookup"><span data-stu-id="73d35-715">An enum type that does not explicitly declare an underlying type has an underlying type of `int`.</span></span> <span data-ttu-id="73d35-716">枚举类型的存储格式和可能的值的范围取决于其基础类型。</span><span class="sxs-lookup"><span data-stu-id="73d35-716">An enum type's storage format and range of possible values are determined by its underlying type.</span></span> <span data-ttu-id="73d35-717">枚举类型可以采用上的值的集不受其枚举成员。</span><span class="sxs-lookup"><span data-stu-id="73d35-717">The set of values that an enum type can take on is not limited by its enum members.</span></span> <span data-ttu-id="73d35-718">具体而言，枚举的基础类型的任何值可以转换为枚举类型，该枚举类型的不同有效值。</span><span class="sxs-lookup"><span data-stu-id="73d35-718">In particular, any value of the underlying type of an enum can be cast to the enum type and is a distinct valid value of that enum type.</span></span>

<span data-ttu-id="73d35-719">下面的示例声明名为枚举类型`Alignment`使用的基础类型为`sbyte`。</span><span class="sxs-lookup"><span data-stu-id="73d35-719">The following example declares an enum type named `Alignment` with an underlying type of `sbyte`.</span></span>

```csharp
enum Alignment: sbyte
{
    Left = -1,
    Center = 0,
    Right = 1
}
```
<span data-ttu-id="73d35-720">上面的示例所示，枚举成员的声明可以包括指定成员的值的常量表达式。</span><span class="sxs-lookup"><span data-stu-id="73d35-720">As shown by the previous example, an enum member declaration can include a constant expression that specifies the value of the member.</span></span> <span data-ttu-id="73d35-721">每个枚举成员的常量值必须是枚举的基础类型范围内。</span><span class="sxs-lookup"><span data-stu-id="73d35-721">The constant value for each enum member must be in the range of the underlying type of the enum.</span></span> <span data-ttu-id="73d35-722">当枚举成员的声明不显式指定一个值时，该成员提供的值为零 （如果它是枚举类型中的第一个成员） 或原文前的枚举成员加上一个值。</span><span class="sxs-lookup"><span data-stu-id="73d35-722">When an enum member declaration does not explicitly specify a value, the member is given the value zero (if it is the first member in the enum type) or the value of the textually preceding enum member plus one.</span></span>

<span data-ttu-id="73d35-723">枚举值可以转换成整型值和使用类型强制转换，反之亦然。</span><span class="sxs-lookup"><span data-stu-id="73d35-723">Enum values can be converted to integral values and vice versa using type casts.</span></span> <span data-ttu-id="73d35-724">例如</span><span class="sxs-lookup"><span data-stu-id="73d35-724">For example</span></span>

```csharp
int i = (int)Color.Blue;        // int i = 2;
Color c = (Color)2;             // Color c = Color.Blue;
```
<span data-ttu-id="73d35-725">任何枚举类型的默认值是整数值转换为枚举类型的零。</span><span class="sxs-lookup"><span data-stu-id="73d35-725">The default value of any enum type is the integral value zero converted to the enum type.</span></span> <span data-ttu-id="73d35-726">在其中变量将自动初始化为默认值的情况下，这是枚举类型的变量指定的值。</span><span class="sxs-lookup"><span data-stu-id="73d35-726">In cases where variables are automatically initialized to a default value, this is the value given to variables of enum types.</span></span> <span data-ttu-id="73d35-727">为了使默认值的枚举类型可供方便使用，文本`0`隐式转换为任何枚举类型。</span><span class="sxs-lookup"><span data-stu-id="73d35-727">In order for the default value of an enum type to be easily available, the literal `0` implicitly converts to any enum type.</span></span> <span data-ttu-id="73d35-728">因此，可以运行以下命令。</span><span class="sxs-lookup"><span data-stu-id="73d35-728">Thus, the following is permitted.</span></span>

```csharp
Color c = 0;
```

## <a name="delegates"></a><span data-ttu-id="73d35-729">委托</span><span class="sxs-lookup"><span data-stu-id="73d35-729">Delegates</span></span>

<span data-ttu-id="73d35-730">***委托类型***表示对具有特定参数列表和返回类型的方法的引用。</span><span class="sxs-lookup"><span data-stu-id="73d35-730">A ***delegate type*** represents references to methods with a particular parameter list and return type.</span></span> <span data-ttu-id="73d35-731">通过委托，可以将方法视为可分配给变量并可作为参数传递的实体。</span><span class="sxs-lookup"><span data-stu-id="73d35-731">Delegates make it possible to treat methods as entities that can be assigned to variables and passed as parameters.</span></span> <span data-ttu-id="73d35-732">委托类似于其他一些语言中的函数指针概念，但与函数指针不同的是，委托不仅面向对象，还类型安全。</span><span class="sxs-lookup"><span data-stu-id="73d35-732">Delegates are similar to the concept of function pointers found in some other languages, but unlike function pointers, delegates are object-oriented and type-safe.</span></span>

<span data-ttu-id="73d35-733">下面的示例声明并使用 `Function` 委托类型。</span><span class="sxs-lookup"><span data-stu-id="73d35-733">The following example declares and uses a delegate type named `Function`.</span></span>

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
<span data-ttu-id="73d35-734">`Function` 委托类型实例可以引用需要使用 `double` 自变量并返回 `double` 值的方法。</span><span class="sxs-lookup"><span data-stu-id="73d35-734">An instance of the `Function` delegate type can reference any method that takes a `double` argument and returns a `double` value.</span></span> <span data-ttu-id="73d35-735">`Apply`方法将应用给定`Function`的元素`double[]`，使其返回`double[]`的结果。</span><span class="sxs-lookup"><span data-stu-id="73d35-735">The `Apply` method applies a given `Function` to the elements of a `double[]`, returning a `double[]` with the results.</span></span> <span data-ttu-id="73d35-736">在 `Main` 方法中，`Apply` 用于向 `double[]` 应用三个不同的函数。</span><span class="sxs-lookup"><span data-stu-id="73d35-736">In the `Main` method, `Apply` is used to apply three different functions to a `double[]`.</span></span>

<span data-ttu-id="73d35-737">委托可以引用静态方法（如上面示例中的 `Square` 或 `Math.Sin`）或实例方法（如上面示例中的 `m.Multiply`）。</span><span class="sxs-lookup"><span data-stu-id="73d35-737">A delegate can reference either a static method (such as `Square` or `Math.Sin` in the previous example) or an instance method (such as `m.Multiply` in the previous example).</span></span> <span data-ttu-id="73d35-738">引用实例方法的委托还会引用特定对象，通过委托调用实例方法时，该对象会变成调用中的 `this`。</span><span class="sxs-lookup"><span data-stu-id="73d35-738">A delegate that references an instance method also references a particular object, and when the instance method is invoked through the delegate, that object becomes `this` in the invocation.</span></span>

<span data-ttu-id="73d35-739">还可以使用匿名函数创建委托，这些函数是便捷创建的“内联方法”。</span><span class="sxs-lookup"><span data-stu-id="73d35-739">Delegates can also be created using anonymous functions, which are "inline methods" that are created on the fly.</span></span> <span data-ttu-id="73d35-740">匿名函数可以查看周围方法的局部变量。</span><span class="sxs-lookup"><span data-stu-id="73d35-740">Anonymous functions can see the local variables of the surrounding methods.</span></span> <span data-ttu-id="73d35-741">因此，上面的乘数示例可以编写更轻松地而无需使用`Multiplier`类：</span><span class="sxs-lookup"><span data-stu-id="73d35-741">Thus, the multiplier example above can be written more easily without using a `Multiplier` class:</span></span>

```csharp
double[] doubles =  Apply(a, (double x) => x * 2.0);
```
<span data-ttu-id="73d35-742">委托的一个有趣且有用的属性是，它不知道也不关心所引用的方法的类；只关心引用的方法是否具有与委托相同的参数和返回类型。</span><span class="sxs-lookup"><span data-stu-id="73d35-742">An interesting and useful property of a delegate is that it does not know or care about the class of the method it references; all that matters is that the referenced method has the same parameters and return type as the delegate.</span></span>

## <a name="attributes"></a><span data-ttu-id="73d35-743">特性</span><span class="sxs-lookup"><span data-stu-id="73d35-743">Attributes</span></span>

<span data-ttu-id="73d35-744">C# 程序中的类型、成员和其他实体支持使用修饰符来控制其行为的某些方面。</span><span class="sxs-lookup"><span data-stu-id="73d35-744">Types, members, and other entities in a C# program support modifiers that control certain aspects of their behavior.</span></span> <span data-ttu-id="73d35-745">例如，方法的可访问性是由 `public`、`protected`、`internal` 和 `private` 修饰符控制。</span><span class="sxs-lookup"><span data-stu-id="73d35-745">For example, the accessibility of a method is controlled using the `public`, `protected`, `internal`, and `private` modifiers.</span></span> <span data-ttu-id="73d35-746">C# 整合了这种能力，以便可以将用户定义类型的声明性信息附加到程序实体，并在运行时检索此类信息。</span><span class="sxs-lookup"><span data-stu-id="73d35-746">C# generalizes this capability such that user-defined types of declarative information can be attached to program entities and retrieved at run-time.</span></span> <span data-ttu-id="73d35-747">程序通过定义和使用***特性***来指定此类额外的声明性信息。</span><span class="sxs-lookup"><span data-stu-id="73d35-747">Programs specify this additional declarative information by defining and using ***attributes***.</span></span>

<span data-ttu-id="73d35-748">以下示例声明了 `HelpAttribute` 特性，可将其附加到程序实体，以提供指向关联文档的链接。</span><span class="sxs-lookup"><span data-stu-id="73d35-748">The following example declares a `HelpAttribute` attribute that can be placed on program entities to provide links to their associated documentation.</span></span>

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
<span data-ttu-id="73d35-749">所有特性类都派生`System.Attribute`.NET Framework 提供的基类。</span><span class="sxs-lookup"><span data-stu-id="73d35-749">All attribute classes derive from the `System.Attribute` base class provided by the .NET Framework.</span></span> <span data-ttu-id="73d35-750">特性的应用方式为，在相关声明前的方括号内指定特性的名称以及任意自变量。</span><span class="sxs-lookup"><span data-stu-id="73d35-750">Attributes can be applied by giving their name, along with any arguments, inside square brackets just before the associated declaration.</span></span> <span data-ttu-id="73d35-751">如果属性的名称以结尾`Attribute`，可以省略该名称的一部分，该属性引用时。</span><span class="sxs-lookup"><span data-stu-id="73d35-751">If an attribute's name ends in `Attribute`, that part of the name can be omitted when the attribute is referenced.</span></span> <span data-ttu-id="73d35-752">例如，可按如下方法使用 `HelpAttribute` 特性。</span><span class="sxs-lookup"><span data-stu-id="73d35-752">For example, the `HelpAttribute` attribute can be used as follows.</span></span>

```csharp
[Help("http://msdn.microsoft.com/.../MyClass.htm")]
public class Widget
{
    [Help("http://msdn.microsoft.com/.../MyClass.htm", Topic = "Display")]
    public void Display(string text) {}
}
```
<span data-ttu-id="73d35-753">此示例附加`HelpAttribute`到`Widget`类，另一个`HelpAttribute`到`Display`类中的方法。</span><span class="sxs-lookup"><span data-stu-id="73d35-753">This example attaches a `HelpAttribute` to the `Widget` class and another `HelpAttribute` to the `Display` method in the class.</span></span> <span data-ttu-id="73d35-754">特性类的公共构造函数控制了将特性附加到程序实体时必须提供的信息。</span><span class="sxs-lookup"><span data-stu-id="73d35-754">The public constructors of an attribute class control the information that must be provided when the attribute is attached to a program entity.</span></span> <span data-ttu-id="73d35-755">可以通过引用特性类的公共读写属性（如上面示例对 `Topic` 属性的引用），提供其他信息。</span><span class="sxs-lookup"><span data-stu-id="73d35-755">Additional information can be provided by referencing public read-write properties of the attribute class (such as the reference to the `Topic` property previously).</span></span>

<span data-ttu-id="73d35-756">下面的示例演示如何在运行时检索给定的程序实体的属性信息使用反射。</span><span class="sxs-lookup"><span data-stu-id="73d35-756">The following example shows how attribute information for a given program entity can be retrieved at run-time using reflection.</span></span>

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
<span data-ttu-id="73d35-757">通过反射请求获得特定特性时，将调用特性类的构造函数（由程序源提供信息），并返回生成的特性实例。</span><span class="sxs-lookup"><span data-stu-id="73d35-757">When a particular attribute is requested through reflection, the constructor for the attribute class is invoked with the information provided in the program source, and the resulting attribute instance is returned.</span></span> <span data-ttu-id="73d35-758">如果是通过属性提供其他信息，那么在特性实例返回前，这些属性会设置为给定值。</span><span class="sxs-lookup"><span data-stu-id="73d35-758">If additional information was provided through properties, those properties are set to the given values before the attribute instance is returned.</span></span>
