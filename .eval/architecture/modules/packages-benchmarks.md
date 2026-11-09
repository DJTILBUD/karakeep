# Module: packages/benchmarks

Automated performance benchmarking and load-testing suite that spins up a local Docker Compose test stack, seeds users, bookmarks, tags, and lists via tRPC, and measures the execution latency and throughput of tRPC queries.

## Key files
- `packages/benchmarks/src/index.ts`: CLI entry point orchestrating container lifecycle, environment configuration, data seeding, and benchmark execution.
- `packages/benchmarks/src/benchmarks.ts`: Defines and runs Tinybench benchmark suites against various tRPC endpoints (filtering, pagination/cursors, search, lists) and outputs results.
- `packages/benchmarks/src/seed.ts`: Provisions test users, tags, lists, and bookmarks concurrently via tRPC mutations and waits for search indexing.
- `packages/benchmarks/src/startContainers.ts`: Handles spinning up and tearing down the Docker Compose test environment on a dynamic port, checking stack health, and capturing service logs.
- `packages/benchmarks/src/trpc.ts`: Constructs configured tRPC clients and handles user signup via the auth endpoint.
- `packages/benchmarks/src/utils.ts`: Utility functions for polling conditions (waitUntil), sleep delays, and formatting durations and numbers.
- `packages/benchmarks/src/log.ts`: Simple console logging helpers for formatted CLI output.
- `packages/benchmarks/setup/html/hello.html`: Static HTML fixture served by Nginx during benchmark runs.

## Public interface
- runBenchmarks(seed: SeedResult, options?: BenchmarkOptions): Promise<BenchmarkRow[]>
- seedData(config: SeedConfig): Promise<SeedResult>
- startContainers(): Promise<RunningContainers>
- getTrpcClient(apiKey?: string): TrpcClient
- signUpUser(input: { name: string; email: string; password: string }): Promise<void>
- waitUntil(fn: () => Promise<boolean>, description: string, timeoutMs?: number, intervalMs?: number): Promise<void>
- sleep(ms: number): Promise<void>
- formatNumber(num: number, fractionDigits?: number): string
- formatMs(ms: number): string
- logStep(title: string): void
- logInfo(message: string): void
- logSuccess(message: string): void
- logWarn(message: string): void

## Dependencies
- tinybench
- p-limit
- @trpc/client
- superjson
- @karakeep/shared
- @karakeep/trpc

## Open questions
- _none_
