# 🚀 GenAI & Agentic AI with .NET — A Practical Roadmap

> **From .NET Developer → AI Engineer → AI Solution Architect**
>
> A simple, visual, step-by-step roadmap for C# and .NET developers learning **Generative AI, LLMs, RAG, Tool Calling, AI Agents, Agentic AI, MCP and Production AI Architecture**.

[![C#](https://img.shields.io/badge/C%23-12%2B-512BD4?logo=csharp&logoColor=white)](https://learn.microsoft.com/dotnet/csharp/)
[![.NET](https://img.shields.io/badge/.NET-8%2B-512BD4?logo=dotnet&logoColor=white)](https://dotnet.microsoft.com/)
[![ASP.NET Core](https://img.shields.io/badge/ASP.NET%20Core-Web%20API-512BD4?logo=dotnet&logoColor=white)](https://learn.microsoft.com/aspnet/core/)
[![Azure](https://img.shields.io/badge/Microsoft%20Azure-0078D4?logo=microsoftazure&logoColor=white)](https://azure.microsoft.com/)
[![GenAI](https://img.shields.io/badge/AI-Generative%20AI-FF6F00)](https://learn.microsoft.com/azure/ai-services/)
[![RAG](https://img.shields.io/badge/AI-RAG-8B5CF6)](./RAG-using-csharp.md)
[![Agentic AI](https://img.shields.io/badge/AI-Agentic%20AI-EC4899)](https://learn.microsoft.com/)
[![MCP](https://img.shields.io/badge/Protocol-MCP-0EA5E9)](https://modelcontextprotocol.io/)

**Keywords:** `C#` `.NET` `DotNet AI` `ASP.NET Core` `Generative AI` `GenAI` `LLM` `RAG` `AI Agents` `Agentic AI` `MCP` `Tool Calling` `Semantic Kernel` `Microsoft.Extensions.AI` `Azure AI` `Azure OpenAI` `Azure AI Search` `AI Architecture` `Enterprise AI` `AI Engineering`

---

# 🎯 Who Is This Guide For?

This roadmap is designed for:

- C# developers
- .NET developers
- ASP.NET Core developers
- Backend engineers
- Software engineers
- Technical leads
- Solution architects
- Enterprise application developers
- Developers moving from traditional software to AI

### The good news 💡

You **do not need to become a data scientist first**.

Your existing skills in:

```text
C#
.NET
APIs
Microservices
Databases
Cloud
Distributed Systems
Architecture
Testing
DevOps
```

are valuable foundations for AI engineering.

---

# 🧭 The Big Picture

Your journey can look like this:

```mermaid
flowchart LR
    A[💻 .NET Developer]
    B[🧠 LLM Applications]
    C[✍️ Prompt Engineering]
    D[🔎 RAG]
    E[🔧 Tool Calling]
    F[🤖 AI Agents]
    G[🧩 Agentic Workflows]
    H[🌐 Multi-Agent Systems]
    I[🏗️ Production AI]

    A --> B --> C --> D --> E --> F --> G --> H --> I

    classDef start fill:#E0F2FE,stroke:#0284C7,stroke-width:3px,color:#111
    classDef learn fill:#EDE9FE,stroke:#7C3AED,stroke-width:2px,color:#111
    classDef advanced fill:#FCE7F3,stroke:#DB2777,stroke-width:2px,color:#111
    classDef prod fill:#DCFCE7,stroke:#16A34A,stroke-width:3px,color:#111

    class A start
    class B,C,D learn
    class E,F,G,H advanced
    class I prod
```

> 🎨 GitHub supports Mermaid diagrams in Markdown. These diagrams use color and directional sequencing for an animated/interactive-looking learning experience, while remaining native GitHub Markdown.

---

# 🧠 Phase 1 — Strengthen Your .NET Foundation

Before jumping into agents, make sure you are comfortable with:

## C#

Learn:

- Classes and interfaces
- Generics
- LINQ
- Collections
- Async/await
- Exception handling
- HTTP clients
- Serialization
- Dependency injection
- Configuration
- Logging
- Unit testing

## ASP.NET Core

Learn:

- REST APIs
- Middleware
- Dependency Injection
- Authentication
- Authorization
- Configuration
- Health checks
- OpenAPI
- Background services
- API versioning

## Architecture

Understand:

- SOLID
- Clean Architecture
- Domain-Driven Design
- CQRS
- Microservices
- Event-driven architecture
- Distributed systems

> ⭐ These skills become extremely important when an AI prototype becomes an enterprise production system.

---

# ☁️ Phase 2 — Learn the Azure Building Blocks

You do not need to memorize every Azure service.

Learn the services that help you **design and operate AI systems**.

| Capability | Azure option |
|---|---|
| Compute | App Service / Container Apps / AKS |
| Storage | Blob Storage |
| Database | Azure SQL / Cosmos DB |
| Search | Azure AI Search |
| Messaging | Azure Service Bus |
| Identity | Microsoft Entra ID |
| Secrets | Azure Key Vault |
| Monitoring | Azure Monitor / Application Insights |
| AI | Azure AI services |
| LLM platform | Azure OpenAI / Azure AI Foundry ecosystem |

---

# 🧠 Phase 3 — Understand Generative AI

Before learning frameworks, understand the fundamentals.

### Learn these concepts

- LLMs
- Tokens
- Context windows
- Transformers
- Embeddings
- Inference
- Temperature
- Structured output
- Tool/function calling
- Multimodal models
- Model selection
- Model limitations

### Basic mental model

```mermaid
flowchart LR
    U[👤 User] --> APP[🟦 Application]
    APP --> LLM[🤖 LLM]

    LLM --> T[📝 Text]
    LLM --> J[📦 Structured Output]
    LLM --> TOOL[🔧 Tool Call]
    LLM --> C[🧠 Context-Based Answer]

    classDef input fill:#E0F2FE,stroke:#0284C7,stroke-width:2px,color:#111
    classDef app fill:#EDE9FE,stroke:#7C3AED,stroke-width:2px,color:#111
    classDef model fill:#FEF3C7,stroke:#F59E0B,stroke-width:2px,color:#111
    classDef output fill:#DCFCE7,stroke:#16A34A,stroke-width:2px,color:#111

    class U input
    class APP app
    class LLM model
    class T,J,TOOL,C output
```

---

# ✍️ Phase 4 — Learn Prompt Engineering

Start with simple prompts.

Then learn:

- System instructions
- User instructions
- Few-shot examples
- Role prompting
- Context injection
- Output constraints
- Structured outputs
- Prompt templates
- Prompt versioning
- Prompt security

Example:

```text
System:
You are an enterprise support assistant.

Rules:
- Use the supplied company documentation.
- Do not invent information.
- If information is unavailable, say so.

Context:
{retrieved_context}

Question:
{question}
```

### Think of a prompt like an API contract

```text
Input
  ↓
Instructions
  ↓
Context
  ↓
Constraints
  ↓
Expected Output
```

---

# 🔎 Phase 5 — Learn RAG

RAG is one of the most important skills for enterprise GenAI.

```mermaid
flowchart LR
    D[📄 Documents] --> X[🔤 Extract]
    X --> C[✂️ Chunk]
    C --> E[🔢 Embed]
    E --> S[(🔎 Search Index)]

    U[👤 Question] --> Q[🧠 Query]
    Q --> S
    S --> R[🎯 Relevant Context]
    R --> L[🤖 LLM]
    L --> A[💬 Grounded Answer]

    classDef docs fill:#FFF7ED,stroke:#F97316,stroke-width:2px,color:#111
    classDef process fill:#EDE9FE,stroke:#7C3AED,stroke-width:2px,color:#111
    classDef store fill:#DCFCE7,stroke:#16A34A,stroke-width:2px,color:#111
    classDef llm fill:#FEF3C7,stroke:#F59E0B,stroke-width:2px,color:#111

    class D docs
    class X,C,E,Q,R process
    class S store
    class L,A llm
```

### .NET focus

Learn to combine:

```text
ASP.NET Core
+
Azure Blob Storage
+
Azure AI Search
+
Azure OpenAI
+
Azure Functions
+
Azure Service Bus
```

👉 Deep dive: **[RAG Using C# and .NET](./RAG-using-csharp.md)**

---

# 🛠️ Phase 6 — Build Your First GenAI Applications

## 🟢 Project 1 — AI Chat API

```text
ASP.NET Core
     ↓
Chat API
     ↓
LLM
     ↓
Response
```

Learn:

- API design
- Dependency injection
- Configuration
- Error handling
- Logging
- Streaming

---

## 🟢 Project 2 — AI Summarizer

```text
Document
   ↓
Prompt
   ↓
LLM
   ↓
Summary
```

Learn:

- Prompt design
- Structured output
- Token management
- Model selection

---

## 🟡 Project 3 — Document Q&A

```text
PDF
 ↓
Blob Storage
 ↓
Ingestion
 ↓
Chunking
 ↓
Embeddings
 ↓
Azure AI Search
 ↓
ASP.NET Core
 ↓
LLM
 ↓
Answer + Sources
```

---

# 🔧 Phase 7 — Learn Tool Calling

An LLM becomes significantly more useful when it can interact with external systems.

### Example

```text
User:
"What is the status of order 123?"

        ↓

LLM
        ↓
getOrderStatus("123")
        ↓
Order API
        ↓
Order Result
        ↓
LLM
        ↓
Human-friendly answer
```

### Possible tools

- Search
- Database
- Calculator
- REST APIs
- CRM
- ERP
- Ticketing system
- Internal business APIs
- File systems
- Enterprise services

---

# 🤖 Phase 8 — Learn AI Agents

A simple agent can be thought of as:

```mermaid
flowchart TB
    U[👤 User] --> A[🤖 AI Agent]
    A --> S[🔎 Search]
    A --> API[🌐 API]
    A --> DB[(🗄️ Database)]
    S --> R[📦 Results]
    API --> R
    DB --> R
    R --> A
    A --> O[💬 Response]

    classDef user fill:#E0F2FE,stroke:#0284C7,stroke-width:2px,color:#111
    classDef agent fill:#FCE7F3,stroke:#DB2777,stroke-width:3px,color:#111
    classDef tool fill:#EDE9FE,stroke:#7C3AED,stroke-width:2px,color:#111
    classDef result fill:#DCFCE7,stroke:#16A34A,stroke-width:2px,color:#111

    class U user
    class A agent
    class S,API,DB tool
    class R,O result
```

Learn:

- Tool use
- State
- Memory
- Context management
- Planning
- Guardrails
- Human approval
- Evaluation
- Failure handling

---

# 🧩 Phase 9 — Learn Agentic AI

Traditional application:

```text
Question → Answer
```

Agentic application:

```text
Goal
 ↓
Understand
 ↓
Plan
 ↓
Select Tool
 ↓
Execute
 ↓
Observe
 ↓
Evaluate
 ↓
Continue / Stop
```

### Example: Customer Support Agent

```mermaid
flowchart TD
    T[🎫 Customer Ticket]
    H[🔎 Customer History]
    K[📚 Knowledge Search]
    E[🧠 Error Analysis]
    P[📡 Product Status]
    R[📝 Recommendation]
    A[👨‍💼 Human Approval]
    U[✅ Update Ticket]

    T --> H --> K --> E --> P --> R --> A --> U

    classDef start fill:#E0F2FE,stroke:#0284C7,stroke-width:2px,color:#111
    classDef ai fill:#FCE7F3,stroke:#DB2777,stroke-width:2px,color:#111
    classDef action fill:#DCFCE7,stroke:#16A34A,stroke-width:2px,color:#111

    class T start
    class H,K,E,P,R ai
    class A,U action
```

The agent is not simply generating text. It is coordinating **context, tools, decisions and actions**.

---


# 💻 C# Hands-On GenAI & Agentic AI Examples

The fastest way to learn AI engineering is to **build each capability as a small .NET component** and then combine them.

---

# Example 1 — Your First LLM Abstraction

Start with an interface rather than coupling the entire application to one model provider.

```csharp
public interface IChatService
{
    Task<string> GenerateAsync(
        string prompt,
        CancellationToken cancellationToken = default);
}
```

Application code now depends on:

```text
IChatService
    ↓
Your provider implementation
    ↓
LLM
```

This makes provider changes and automated testing easier.

---

# Example 2 — Simple ASP.NET Core AI Endpoint

```csharp
public sealed record ChatRequest(string Message);

[ApiController]
[Route("api/chat")]
public sealed class ChatController : ControllerBase
{
    private readonly IChatService _chat;

    public ChatController(IChatService chat)
    {
        _chat = chat;
    }

    [HttpPost]
    public async Task<IActionResult> Chat(
        [FromBody] ChatRequest request,
        CancellationToken cancellationToken)
    {
        if (string.IsNullOrWhiteSpace(request.Message))
        {
            return BadRequest("Message is required.");
        }

        var answer = await _chat.GenerateAsync(
            request.Message,
            cancellationToken);

        return Ok(new
        {
            answer
        });
    }
}
```

You have now created a basic:

```text
HTTP Request
     ↓
ASP.NET Core
     ↓
IChatService
     ↓
LLM
     ↓
HTTP Response
```

---

# Example 3 — Prompt Template in C#

Keep prompts out of controller code.

```csharp
public static class SupportPrompt
{
    public static string Build(
        string context,
        string question)
    {
        return $"""
        You are an enterprise support assistant.

        Rules:
        - Use the supplied context.
        - Do not invent information.
        - If the answer is unavailable, say so.

        Context:
        {context}

        Question:
        {question}
        """;
    }
}
```

This makes prompts:

- Testable
- Versionable
- Reusable
- Easier to review

---

# Example 4 — Structured Output

Suppose you want the model to classify a support ticket.

```csharp
public sealed record TicketClassification(
    string Category,
    string Priority,
    double Confidence);
```

Your application should validate the returned structure before using it.

```csharp
public static bool IsValid(
    TicketClassification result)
{
    var categories = new[]
    {
        "Billing",
        "Technical",
        "Account",
        "Other"
    };

    var priorities = new[]
    {
        "Low",
        "Medium",
        "High",
        "Critical"
    };

    return categories.Contains(result.Category)
        && priorities.Contains(result.Priority)
        && result.Confidence is >= 0 and <= 1;
}
```

> Structured output reduces ambiguity, but **your application must still validate the result**.

---

# Example 5 — Add RAG to the Chat Application

Combine the previous concepts.

```csharp
public sealed class EnterpriseAssistant
{
    private readonly IRetrievalService _retrieval;
    private readonly IChatService _chat;

    public EnterpriseAssistant(
        IRetrievalService retrieval,
        IChatService chat)
    {
        _retrieval = retrieval;
        _chat = chat;
    }

    public async Task<string> AskAsync(
        string question,
        CancellationToken cancellationToken = default)
    {
        var chunks = await _retrieval.SearchAsync(
            question,
            topK: 5,
            cancellationToken);

        var context = string.Join(
            "\n\n",
            chunks.Select(x => x.Content));

        var prompt = $"""
        Answer using only the supplied context.

        Context:
        {context}

        Question:
        {question}

        If the answer is not in the context,
        say that the information is unavailable.
        """;

        return await _chat.GenerateAsync(
            prompt,
            cancellationToken);
    }
}
```

Now:

```text
User
 ↓
ASP.NET Core
 ↓
EnterpriseAssistant
 ├── Search
 └── LLM
 ↓
Grounded Answer
```

For the deeper RAG implementation, see **[RAG Using C# and .NET](./RAG-using-csharp.md)**.

---

# Example 6 — Define a Tool

A tool should have:

1. A name
2. A description
3. Input parameters
4. An implementation
5. Authorization rules

Example:

```csharp
public sealed record Order(
    string Id,
    string Status,
    decimal Amount);

public interface IOrderService
{
    Task<Order?> GetOrderAsync(
        string orderId,
        CancellationToken cancellationToken = default);
}
```

Tool wrapper:

```csharp
public sealed class OrderTools
{
    private readonly IOrderService _orders;

    public OrderTools(IOrderService orders)
    {
        _orders = orders;
    }

    public async Task<Order?> GetOrderStatusAsync(
        string orderId,
        CancellationToken cancellationToken = default)
    {
        return await _orders.GetOrderAsync(
            orderId,
            cancellationToken);
    }
}
```

Conceptually:

```text
LLM
 ↓
getOrderStatus("123")
 ↓
OrderTools
 ↓
IOrderService
 ↓
Order API / Database
 ↓
Order
 ↓
LLM
 ↓
Human-readable answer
```

---

# Example 7 — Validate Tool Arguments

Never blindly execute model-generated arguments.

```csharp
public static bool IsValidOrderId(string orderId)
{
    return !string.IsNullOrWhiteSpace(orderId)
        && orderId.Length <= 50
        && orderId.All(char.IsLetterOrDigit);
}
```

Before execution:

```csharp
if (!IsValidOrderId(orderId))
{
    throw new ArgumentException(
        "Invalid order ID.",
        nameof(orderId));
}
```

For sensitive operations, also validate:

```text
User Identity
     ↓
Permission
     ↓
Tool Permission
     ↓
Input Validation
     ↓
Tool Execution
```

---

# Example 8 — A Simple Agent Loop

An agent can be understood as a loop:

```text
Goal
 ↓
Think / Decide
 ↓
Select Tool
 ↓
Execute
 ↓
Observe
 ↓
Decide Again
 ↓
Finish
```

A simplified C# orchestration model:

```csharp
public sealed class AgentRunner
{
    private readonly IChatService _chat;
    private readonly IToolRegistry _tools;

    public AgentRunner(
        IChatService chat,
        IToolRegistry tools)
    {
        _chat = chat;
        _tools = tools;
    }

    public async Task<string> RunAsync(
        string goal,
        CancellationToken cancellationToken = default)
    {
        const int maxIterations = 5;

        var state = new AgentState(goal);

        for (var i = 0; i < maxIterations; i++)
        {
            var decision = await _chat.GenerateAsync(
                state.BuildPrompt(),
                cancellationToken);

            if (decision.StartsWith("FINAL:", StringComparison.OrdinalIgnoreCase))
            {
                return decision["FINAL:".Length..].Trim();
            }

            var toolCall = ToolCallParser.Parse(decision);

            if (toolCall is null)
            {
                return "The agent could not produce a valid action.";
            }

            var result = await _tools.ExecuteAsync(
                toolCall,
                cancellationToken);

            state.AddObservation(
                toolCall,
                result);
        }

        return "The agent reached its execution limit.";
    }
}
```

This is intentionally simplified. Production agents need stronger structured tool calls, state handling, permissions, retries, timeouts, tracing, evaluation and safety controls.

---

# Example 9 — Agent State

Keep state explicit.

```csharp
public sealed class AgentState
{
    private readonly List<string> _observations = new();

    public AgentState(string goal)
    {
        Goal = goal;
    }

    public string Goal { get; }

    public IReadOnlyList<string> Observations =>
        _observations;

    public void AddObservation(
        ToolCall call,
        string result)
    {
        _observations.Add(
            $"Tool: {call.Name}\nResult: {result}");
    }

    public string BuildPrompt()
    {
        var observations = string.Join(
            "\n\n",
            _observations);

        return $"""
        Goal:
        {Goal}

        Previous observations:
        {observations}

        Decide the next action.
        """;
    }
}
```

This demonstrates an important agent concept:

> **An agent is not just a prompt. It is a stateful orchestration loop.**

---

# Example 10 — Tool Registry

Keep tools discoverable and centralized.

```csharp
public interface IToolRegistry
{
    Task<string> ExecuteAsync(
        ToolCall call,
        CancellationToken cancellationToken);
}
```

Example implementation:

```csharp
public sealed class ToolRegistry : IToolRegistry
{
    private readonly OrderTools _orders;

    public ToolRegistry(OrderTools orders)
    {
        _orders = orders;
    }

    public async Task<string> ExecuteAsync(
        ToolCall call,
        CancellationToken cancellationToken)
    {
        return call.Name switch
        {
            "getOrderStatus" =>
                await ExecuteOrderStatusAsync(
                    call,
                    cancellationToken),

            _ => throw new InvalidOperationException(
                $"Unknown tool: {call.Name}")
        };
    }

    private async Task<string> ExecuteOrderStatusAsync(
        ToolCall call,
        CancellationToken cancellationToken)
    {
        var orderId = call.Arguments["orderId"];

        var order = await _orders.GetOrderStatusAsync(
            orderId,
            cancellationToken);

        return order is null
            ? "Order not found."
            : $"Order {order.Id} is {order.Status}.";
    }
}
```

---

# Example 11 — Human Approval for Dangerous Actions

Not every tool call should execute automatically.

```csharp
public enum RiskLevel
{
    Low,
    Medium,
    High,
    Critical
}
```

Example policy:

```csharp
public static bool RequiresHumanApproval(
    string toolName,
    RiskLevel risk)
{
    if (risk is RiskLevel.High or RiskLevel.Critical)
    {
        return true;
    }

    return toolName switch
    {
        "deleteCustomer" => true,
        "issueRefund" => true,
        "deployProduction" => true,
        _ => false
    };
}
```

Workflow:

```text
Agent
 ↓
Tool Request
 ↓
Risk Check
 ├── Low → Execute
 └── High → Human Approval
                 ↓
              Execute
```

This pattern is extremely important for enterprise Agentic AI.

---

# Example 12 — MCP-Friendly Tool Design

When exposing capabilities through a protocol such as MCP, design tools with clear contracts.

```csharp
public sealed record SearchDocumentsRequest(
    string Query,
    int TopK);

public sealed record SearchDocumentsResponse(
    IReadOnlyList<DocumentChunk> Results);
```

The underlying business logic can remain independent:

```text
MCP Adapter
     ↓
Application Interface
     ↓
Domain / Business Logic
     ↓
Infrastructure
```

This keeps protocol concerns out of your core domain.

---

# Example 13 — Dependency Injection for AI Components

```csharp
var builder = WebApplication.CreateBuilder(args);

builder.Services.AddControllers();

builder.Services.AddScoped<IChatService, ChatService>();
builder.Services.AddScoped<IEmbeddingService, EmbeddingService>();
builder.Services.AddScoped<IRetrievalService, AzureSearchRetrievalService>();

builder.Services.AddScoped<IOrderService, OrderService>();
builder.Services.AddScoped<OrderTools>();
builder.Services.AddScoped<IToolRegistry, ToolRegistry>();
builder.Services.AddScoped<AgentRunner>();

var app = builder.Build();

app.MapControllers();

app.Run();
```

A clean dependency graph:

```text
Controller
    ↓
Application Service
    ├── Chat
    ├── Retrieval
    └── Tools
          ↓
     Infrastructure
```

---

# Example 14 — Add Cancellation and Timeouts

AI requests can be slow or expensive.

```csharp
using var timeout =
    CancellationTokenSource.CreateLinkedTokenSource(
        cancellationToken);

timeout.CancelAfter(TimeSpan.FromSeconds(30));

var answer = await _chat.GenerateAsync(
    prompt,
    timeout.Token);
```

For production, also consider:

- Retries with backoff
- Circuit breakers
- Rate limits
- Concurrency limits
- Token budgets
- Model fallbacks

---

# Example 15 — Log AI Operations

Never log sensitive prompts blindly.

```csharp
_logger.LogInformation(
    "AI request started. Operation={Operation}, User={UserId}",
    "RAG",
    userId);
```

Track useful metadata:

```text
Request ID
User / Tenant
Model
Latency
Input tokens
Output tokens
Retrieved documents
Tool calls
Errors
Cost estimate
```

Avoid logging secrets, credentials and unnecessary PII.

---

# 🧪 Build the Learning Projects in This Order

```mermaid
flowchart TD
    A[💬 AI Chat API]
    B[📝 AI Summarizer]
    C[🔎 RAG Application]
    D[🔧 Tool Calling]
    E[🤖 Single Agent]
    F[🧩 Agentic Workflow]
    G[🔗 MCP Tools]
    H[🏢 Enterprise AI Platform]

    A --> B --> C --> D --> E --> F --> G --> H

    classDef beginner fill:#E0F2FE,stroke:#0284C7,stroke-width:2px,color:#111
    classDef intermediate fill:#EDE9FE,stroke:#7C3AED,stroke-width:2px,color:#111
    classDef advanced fill:#FCE7F3,stroke:#DB2777,stroke-width:2px,color:#111
    classDef architect fill:#DCFCE7,stroke:#16A34A,stroke-width:3px,color:#111

    class A,B beginner
    class C,D intermediate
    class E,F,G advanced
    class H architect
```

---

# 🏆 What You Are Actually Learning

Do not memorize the code. Understand the architecture:

```text
C# / .NET
    ↓
API
    ↓
LLM
    ↓
Context
    ↓
RAG
    ↓
Tools
    ↓
Agent
    ↓
State
    ↓
Orchestration
    ↓
Security
    ↓
Evaluation
    ↓
Observability
    ↓
Production
```

The goal is to become a **.NET engineer who can design AI systems**, not merely someone who knows how to call an LLM.


# 🔗 Phase 10 — Learn AI Protocols

Explore:

- Model Context Protocol (MCP)
- Agent-to-Agent communication
- Tool interfaces
- Resource discovery
- Structured tool schemas

### Why protocols matter

Imagine every application exposing tools in a different format.

```text
Agent A → Custom Tool Format
Agent B → Another Format
Agent C → Another Format
```

Protocols create a more consistent way to expose capabilities.

---

# 🧠 Phase 11 — Learn .NET AI Frameworks

Do not learn every framework simultaneously.

Start with the fundamentals.

## Microsoft / .NET ecosystem

Explore:

- Azure AI
- Azure OpenAI
- Azure AI Search
- Azure AI Foundry ecosystem
- Semantic Kernel
- Microsoft.Extensions.AI

## Broader ecosystem

Understand the ideas behind:

- LangChain
- LangGraph
- LlamaIndex
- AutoGen
- CrewAI

### The real skill

Do not memorize frameworks.

Understand:

> **Models + Context + Retrieval + Tools + State + Orchestration**

---

# 🏗️ Phase 12 — Production AI Architecture

A production system needs more than an LLM.

```mermaid
flowchart TB
    U[👥 Users] --> GW[🌐 API Gateway]
    GW --> API[🟦 ASP.NET Core]

    API --> RAG[🔎 RAG]
    API --> AG[🤖 Agent]
    API --> B[🏢 Business APIs]

    RAG --> SEARCH[(Azure AI Search)]
    AG --> TOOLS[🔧 Tools]
    B --> DB[(🗄️ Enterprise Data)]

    RAG --> LLM[🧠 LLM]
    TOOLS --> LLM
    B --> LLM

    LLM --> G[🛡️ Guardrails]
    G --> O[💬 Response]

    OBS[📊 Observability] -.-> API
    OBS -.-> LLM
    SEC[🔐 Identity / Security] -.-> API

    classDef user fill:#E0F2FE,stroke:#0284C7,stroke-width:2px,color:#111
    classDef app fill:#EDE9FE,stroke:#7C3AED,stroke-width:2px,color:#111
    classDef ai fill:#FEF3C7,stroke:#F59E0B,stroke-width:2px,color:#111
    classDef secure fill:#DCFCE7,stroke:#16A34A,stroke-width:2px,color:#111
    classDef infra fill:#F3E8FF,stroke:#9333EA,stroke-width:2px,color:#111

    class U user
    class GW,API,RAG,AG,B app
    class LLM,G,O ai
    class SEARCH,TOOLS,DB infra
    class OBS,SEC secure
```

Supporting capabilities may include:

- Identity
- Key Vault
- Storage
- Service Bus
- Databases
- Search
- Monitoring
- Containers
- CI/CD
- Evaluation
- Cost controls

---

# 🔐 Phase 13 — AI Security

Learn:

- Prompt injection
- Jailbreaks
- Data leakage
- Excessive tool permissions
- Malicious documents
- PII exposure
- Cross-tenant leakage
- Secret exposure
- Output validation
- Authorization
- Auditability

> ⚠️ **Treat model output and retrieved content as untrusted input.**

Traditional application security still matters. AI introduces another attack surface.

---

# 📊 Phase 14 — AI Evaluation

## RAG evaluation

Measure:

- Retrieval relevance
- Context relevance
- Groundedness
- Citation quality
- Answer correctness

## Agent evaluation

Measure:

- Task completion
- Tool selection
- Tool-call correctness
- Failure recovery
- Cost
- Latency
- Safety

### Golden dataset

```text
Input
 ↓
Expected behavior
 ↓
Run application
 ↓
Compare result
 ↓
Score
 ↓
Track regression
```

> 🧪 **Evaluation should become part of your development lifecycle, not a final demo activity.**

---

# 💰 Phase 15 — AI Cost Optimization

Think about every cost-producing operation:

```text
Input Tokens
+
Output Tokens
+
Embedding Calls
+
Search
+
Tool Calls
+
Infrastructure
=
💰 Total Cost
```

Optimization techniques:

- Smaller models for simple tasks
- Better retrieval
- Smaller context
- Prompt optimization
- Caching
- Batching
- Model routing
- Tool-call limits
- Token budgets

---

# ⚙️ Phase 16 — Observability

Track:

```text
Request
 ├── API latency
 ├── Retrieval latency
 ├── Search quality
 ├── LLM latency
 ├── Input tokens
 ├── Output tokens
 ├── Tool calls
 ├── Errors
 ├── Retries
 ├── Cost
 └── User feedback
```

Example:

```text
Request
  ├── Retrieval: 120 ms
  ├── Search: 80 ms
  ├── LLM: 1.8 sec
  ├── Tool Call: 250 ms
  └── Total: 2.3 sec
```

---

# 🧪 Hands-On Project Roadmap

## 🟢 Beginner

### Project 1 — AI Chat API

Learn:

- LLM integration
- ASP.NET Core
- Dependency Injection
- Configuration

### Project 2 — AI Text Summarizer

Learn:

- Prompt engineering
- Structured responses
- Token management

---

## 🟡 Intermediate

### Project 3 — Document Q&A RAG

Learn:

- Document ingestion
- Embeddings
- Azure AI Search
- Retrieval
- Grounding

### Project 4 — Enterprise Knowledge Assistant

Add:

- Authentication
- Authorization
- Citations
- Metadata filters

---

## 🟠 Advanced

### Project 5 — AI Agent with Tools

Build tools for:

- Search
- Database
- REST APIs
- Calculations

### Project 6 — Agentic Customer Support

```text
Customer Request
      ↓
Triage Agent
      ↓
Knowledge Agent
      ↓
Customer Data Agent
      ↓
Resolution Agent
      ↓
Human Approval
      ↓
Action
```

---

## 🔴 Architect Level

### Project 7 — Enterprise Agentic AI Platform

Include:

```text
Multi-Agent Orchestration
        +
RAG
        +
MCP
        +
Identity / RBAC
        +
Guardrails
        +
Evaluation
        +
Observability
        +
Cost Controls
        +
Human-in-the-Loop
        +
Event-Driven Architecture
        +
CI/CD
```

---

# 🗓️ 6-Month Learning Roadmap

| Month | Focus | Build |
|---|---|---|
| 1 | C#, ASP.NET Core, Azure | AI Chat API |
| 2 | LLMs, tokens, prompting, embeddings | AI Summarizer |
| 3 | RAG, Azure AI Search, LLM integration | Document Q&A |
| 4 | Tool calling, agents, .NET AI | Tool-using Agent |
| 5 | Agentic AI, MCP, evaluation, security | Agentic Workflow |
| 6 | Architecture, observability, cost | Enterprise Capstone |

---

# 📚 Recommended Learning Sequence

```text
01. C# / .NET
        ↓
02. ASP.NET Core
        ↓
03. Azure
        ↓
04. LLM Fundamentals
        ↓
05. Prompt Engineering
        ↓
06. Embeddings
        ↓
07. RAG
        ↓
08. Azure AI Search
        ↓
09. LLM Integration
        ↓
10. Tool Calling
        ↓
11. AI Agents
        ↓
12. Semantic Kernel / .NET AI
        ↓
13. MCP
        ↓
14. Agentic AI
        ↓
15. Evaluation + Security
        ↓
16. Production AI Architecture
```

---

# 🏆 Final Capstone — Enterprise AI Assistant for .NET

Build one serious project that demonstrates everything.

```mermaid
flowchart TB
    U[👤 User] --> UI[🖥️ Web / API]
    UI --> AUTH[🔐 Identity + RBAC]
    AUTH --> ORCH[🧠 AI Orchestrator]

    ORCH --> RAG[🔎 RAG]
    ORCH --> AG[🤖 Agent]
    ORCH --> MCP[🔗 MCP Tools]
    ORCH --> BIZ[🏢 Business APIs]

    RAG --> SEARCH[(🔍 AI Search)]
    AG --> LLM[🧠 LLM]
    MCP --> LLM
    BIZ --> DATA[(🗄️ Enterprise Data)]

    LLM --> G[🛡️ Guardrails]
    G --> E[🧪 Evaluation]
    E --> O[📊 Observability]
    O --> OUT[💬 Trusted Response]

    classDef user fill:#E0F2FE,stroke:#0284C7,stroke-width:2px,color:#111
    classDef core fill:#EDE9FE,stroke:#7C3AED,stroke-width:2px,color:#111
    classDef ai fill:#FEF3C7,stroke:#F59E0B,stroke-width:3px,color:#111
    classDef secure fill:#DCFCE7,stroke:#16A34A,stroke-width:2px,color:#111
    classDef data fill:#FCE7F3,stroke:#DB2777,stroke-width:2px,color:#111

    class U,UI user
    class AUTH,ORCH,RAG,AG,MCP,BIZ core
    class LLM,G,E,OUT ai
    class O secure
    class SEARCH,DATA data
```

Your capstone should demonstrate:

- C#
- ASP.NET Core
- Azure AI
- RAG
- Tool Calling
- AI Agents
- MCP
- Authentication
- Authorization
- Guardrails
- Evaluation
- Observability
- Cost Management
- Production architecture

---

# 💼 Career Path

```text
.NET Developer
      ↓
Senior .NET Developer
      ↓
AI Application Developer
      ↓
GenAI Engineer
      ↓
AI Engineer
      ↓
Senior AI Engineer
      ↓
AI Solution Architect
      ↓
Principal AI Engineer / AI Architect
```

Your advantage as an experienced .NET engineer is that you already understand **software engineering**.

Now add:

> **LLMs + RAG + Tools + Agents + AI Architecture**

---

# 🚀 What You Should Be Able to Build

After following this roadmap, you should be able to design and build:

- 💬 AI chat applications
- 📄 Document intelligence systems
- 🔎 Enterprise RAG systems
- 🧠 AI-powered search
- 📚 Knowledge assistants
- 🤖 AI copilots
- 🔧 Tool-using agents
- 🧩 Agentic workflows
- 🌐 Multi-agent systems
- 🏢 Enterprise AI platforms

---

# ⭐ The Most Important Advice

Do **not** try to learn every AI framework.

Instead, master the concepts:

```text
Models
  ↓
Context
  ↓
Prompting
  ↓
Embeddings
  ↓
Retrieval
  ↓
RAG
  ↓
Tools
  ↓
Agents
  ↓
Agentic Workflows
  ↓
Security
  ↓
Evaluation
  ↓
Observability
  ↓
Production Architecture
```

Then implement those concepts using the ecosystem you already know:

> **C# + .NET + Azure**

---

# 🔥 Start Here

### Step 1

Read:

**[RAG Using C# and .NET](./RAG-using-csharp.md)**

### Step 2

Build:

**ASP.NET Core + Azure AI Search + RAG + Citations**

### Step 3

Add:

**Tool Calling**

### Step 4

Add:

**AI Agent**

### Step 5

Add:

**MCP + Guardrails + Evaluation + Observability**

### Step 6

Turn it into:

> 🏆 **A production-ready Enterprise Agentic AI platform**

---

## 🔎 SEO / GitHub Keywords

`dotnet-ai` `csharp-ai` `dotnet-genai` `csharp-genai` `generative-ai-dotnet` `agentic-ai-dotnet` `ai-agents-csharp` `rag-dotnet` `rag-csharp` `mcp-dotnet` `model-context-protocol` `semantic-kernel` `microsoft-extensions-ai` `azure-ai` `azure-openai` `azure-ai-search` `llm` `genai` `generative-ai` `agentic-ai` `ai-engineering` `ai-architecture` `enterprise-ai` `aspnet-core` `ai-solution-architect`
