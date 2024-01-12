<!--DO NOT EDIT : this file has been generated-->

# Reports

> Code quality reports

## Metrics

<div class="chart-container" style="float:right; height:450px; width:450px">
    <canvas id="metricsChart"></canvas>
</div>

| Files | 7 | |
| ----- | -: | - |
| Lines of code | 1299 | (w/o comments) |
| Comments | 1177 | (+ 130 with code) |
| Empty lines | 163 | |
| **Total lines** | **2630** | (w/o tests) |
| TODO | 0 | lines |
| Tests | 3278 | (w/o comments) |

<script>
var ctx = document.getElementById('metricsChart');
var myChart = new Chart(ctx, {
    type: 'pie',
    data: {
        labels: ['Code', 'Comments', 'Empty', 'Tests'],
        datasets: [{
            label: 'Metrics',
            data: [1299, 
                1177, 
                163,
                3278
            ],
            backgroundColor: [
                'rgba(255, 99, 132, 0.2)',
                'rgba(54, 162, 235, 0.2)',
                'rgba(255, 206, 86, 0.2)',
                'rgba(75, 192, 192, 0.2)',
                'rgba(153, 102, 255, 0.2)',
                'rgba(255, 159, 64, 0.2)'
            ],
            borderColor: [
                'rgba(255,99,132,1)',
                'rgba(54, 162, 235, 1)',
                'rgba(255, 206, 86, 1)',
                'rgba(75, 192, 192, 1)',
                'rgba(153, 102, 255, 1)',
                'rgba(255, 159, 64, 1)'
            ],
            borderWidth: 2
        }]
    }
});
</script>

## Linter

**❌ &nbsp; 6 problems**


| File | Position | Severity | Rule | Failure |
| ---- | --- | -------- | ---- | ------- |
| `base.ts` | 85,21-35 | 🌧 | no-prototype-builtins | Do not access Object.prototype method 'hasOwnProperty' from target object. |
| `namespace.ts` | 165,28-42 | 🌧 | no-prototype-builtins | Do not access Object.prototype method 'hasOwnProperty' from target object. |
| `namespace.ts` | 173,16-30 | 🌧 | no-prototype-builtins | Do not access Object.prototype method 'hasOwnProperty' from target object. |
| `namespace.ts` | 196,32-46 | 🌧 | no-prototype-builtins | Do not access Object.prototype method 'hasOwnProperty' from target object. |
| `namespace.ts` | 218,32-46 | 🌧 | no-prototype-builtins | Do not access Object.prototype method 'hasOwnProperty' from target object. |
| `namespace.ts` | 393,20-29 | 🌧 | prefer-rest-params | Use the rest parameters instead of 'arguments'. |



## Tests

|   | Tests suites | Tests |
| - | ------------ | ----- |
| ❌ &nbsp; Failed | 0 | 0 |
| ✅ &nbsp; Passed | 14 | 181 |
| ✴ &nbsp; Pending | 0 | 0 |
| ☢ &nbsp; Error | 0 | |
| **Total** | **14** | **181** |




### ✅ `/test/reviver.test.ts` **2.036s**  <!-- {docsify-ignore} -->


#### 🔹 Operations with Revivers

| Status | Suite | Test |
| ------ | ----- | ---- |
| ✅ | Revive object | stringify reviver |
| ✅ | Revive object | reviver from JSON |
| ✅ | Revive object | reviver from replacer |
| ✅ | Revive class | stringify reviver |
| ✅ | Revive class | reviver from JSON |
| ✅ | Revive class | reviver from replacer |
| ✅ | Revive class with namespace | stringify reviver |
| ✅ | Revive class with namespace | reviver from JSON |
| ✅ | Revive class with namespace | reviver from replacer |
| ✅ | Nested reviver | stringify reviver |


#### 🔹 Revivers generation

| Status | Suite | Test |
| ------ | ----- | ---- |
| ✅ | Arrays | single item |
| ✅ | Arrays | 2 items |
| ✅ | Arrays | 3 items |
| ✅ | Arrays | n items |
| ✅ | Deep struct in arrays | single item |
| ✅ | Deep struct in arrays | 2 items |
| ✅ | Deep struct in arrays | 3 items |
| ✅ | Deep struct in arrays | n items |
| ✅ | Tuple | single mapping |
| ✅ | Range | [1-2] |
| ✅ | Range | [1-3] |
| ✅ | Range | [1-10] |
| ✅ | Tuple | Mix |
| ✅ | Ranges | with RegExp inside |
| ✅ | Submapper | can merge |
| ✅ | Submapper | with primitive inside |
| ✅ | Submapper | with primitive before |
| ✅ | Submapper | with primitive after |
| ✅ | Merge reviver | Missing mapping after |
| ✅ | Merge reviver | Missing mapping before |
| ✅ | Merge reviver | Disjoints mappings |
| ✅ | Subrevivers | expect submapper of "Foo" to be {".": "Foo"} |
| ✅ | Subrevivers | submapper gives Jsonizer.Self.Identity |


#### 🔹 Use cases

| Status | Suite | Test |
| ------ | ----- | ---- |
| ✅ |  | .map() to a reviver |
| ✅ |  | a reviver can handle both an array or an object |



### ✅ `/test/userGuide.test.ts` **2.199s**  <!-- {docsify-ignore} -->


#### 🔹 USER_GUIDE.md examples

| Status | Suite | Test |
| ------ | ----- | ---- |
| ✅ | Overview | Invariants |
| ✅ | Overview | w/o Jsonizer |
| ✅ | Overview | with Jsonizer |
| ✅ | Revivers mappings | Objects |
| ✅ | Revivers mappings | Arrays |
| ✅ | Revivers mappings | Nested mapping |
| ✅ | Revivers mappings | Tuples |
| ✅ | Classes | Custom classes |
| ✅ | Classes | Self apply |
| ✅ | Classes | Self assign |
| ✅ | Classes | No @ decorator |
| ✅ | Classes | Class with nested JSON |
| ✅ | Classes | Class with nested class |
| ✅ | Classes | Pass through (Identity) |
| ✅ | Classes | Errors |
| ✅ | Classes | The `.` (self) builder |
| ✅ | DTO | `toJSON()` and DTO |
| ✅ | DTO | Types ambivalence |
| ✅ | DTO | Mappers for Sub-DTO |
| ✅ | DTO | Mappers for Sub-DTO (alt) |
| ✅ | DTO | Reviving third-party classes and built-in classes |
| ✅ | DTO | `[Jsonizer.toJSON]` |
| ✅ | DTO | Fixing a bad structure |
| ✅ | Ranges and Regexp | Regexp |
| ✅ | Ranges and Regexp | Regexp (alt) |
| ✅ | Ranges and Regexp | Range |
| ✅ | Namespaces | Jsonizer namespaces |
| ✅ | Namespaces | Jsonizer namespaces (Summary) |
| ✅ | Reviving parsed data | Revive after parsing |
| ✅ | Reviver generation 🔹 Replacer | from class |
| ✅ | Reviver generation 🔹 Replacer | from array |
| ✅ | Reviver generation 🔹 Replacer | from nested structure |
| ✅ | Reviver generation 🔹 Subreviver | Array |
| ✅ | Reviver generation 🔹 Subreviver | Item |
| ✅ | Reviver generation | Dynamic reviver |
| ✅ | Reviver generation 🔹 Plain object with `toJSON()` | revived with Jsonizer.reviver |
| ✅ | Reviver generation 🔹 Plain object with `toJSON()` | revived with a placeholder class |
| ✅ | Reviver generation 🔹 Plain object with `toJSON()` | variant |



### ✅ `/test/basic.test.ts` **2.302s**  <!-- {docsify-ignore} -->


#### 🔹 Stringify with Jsonizer.replacer() gives the expected mapper

| Status | Suite | Test |
| ------ | ----- | ---- |
| ✅ | with built-in type | Date |
| ✅ | with built-in type | [Date] |
| ✅ | with built-in type | {d: Date} |
| ✅ | with custom class | Foo |
| ✅ | with custom class | [Foo] |
| ✅ | with custom class | {f: Foo} |
| ✅ | with 3rd party class | Buffer |
| ✅ | with 3rd party class | [Buffer] |
| ✅ | with 3rd party class | {b: Buffer} |


#### 🔹 Parse with generated reviver gives the expected type hierarchy

| Status | Suite | Test |
| ------ | ----- | ---- |
| ✅ | with built-in type | Date |
| ✅ | with built-in type | [Date] |
| ✅ | with built-in type | {d: Date} |
| ✅ | with custom class | Foo |
| ✅ | with custom class | [Foo] |
| ✅ | with custom class | {f: Foo} |
| ✅ | with 3rd party class | Buffer |
| ✅ | with 3rd party class | [Buffer] |
| ✅ | with 3rd party class | {b: Buffer} |


#### 🔹 Revive after parse gives the expected type hierarchy

| Status | Suite | Test |
| ------ | ----- | ---- |
| ✅ | with built-in type | Date |
| ✅ | with built-in type | [Date] |
| ✅ | with built-in type | {d: Date} |
| ✅ | with custom class | Foo |
| ✅ | with custom class | [Foo] |
| ✅ | with custom class | {f: Foo} |
| ✅ | with 3rd party class | Buffer |
| ✅ | with 3rd party class | [Buffer] |
| ✅ | with 3rd party class | {b: Buffer} |


#### 🔹 Parse/stringify with core JSON types

| Status | Suite | Test |
| ------ | ----- | ---- |
| ✅ | null | Invariant |
| ✅ | null | Stringify |
| ✅ | null | Parse |
| ✅ | null | Revive after parse |
| ✅ | 42 | Invariant |
| ✅ | 42 | Stringify |
| ✅ | 42 | Parse |
| ✅ | 42 | Revive after parse |
| ✅ | true | Invariant |
| ✅ | true | Stringify |
| ✅ | true | Parse |
| ✅ | true | Revive after parse |
| ✅ | false | Invariant |
| ✅ | false | Stringify |
| ✅ | false | Parse |
| ✅ | false | Revive after parse |
| ✅ | "string" | Invariant |
| ✅ | "string" | Stringify |
| ✅ | "string" | Parse |
| ✅ | "string" | Revive after parse |
| ✅ | [] | Invariant |
| ✅ | [] | Stringify |
| ✅ | [] | Parse |
| ✅ | [] | Revive after parse |
| ✅ | {} | Invariant |
| ✅ | {} | Stringify |
| ✅ | {} | Parse |
| ✅ | {} | Revive after parse |
| ✅ | undefined | Invariant |
| ✅ | undefined | Stringify |
| ✅ | Nested structure | Stringify |
| ✅ | Nested structure | Parse |
| ✅ | Nested structure | Revive after parse |
| ✅ | Invariants | API |
| ✅ | Clone | {d: Date} |
| ✅ | Clone | {n: 42} |


#### 🔹 Corner cases

| Status | Suite | Test |
| ------ | ----- | ---- |
| ✅ |  | `null` Reviver |
| ✅ |  | Stringify `[undefined, undefined]` |
| ✅ |  | Nested `[[[Date]]]` |


#### 🔹 @Namespace gives a qualified name to classes

| Status | Suite | Test |
| ------ | ----- | ---- |
| ✅ |  | Chain |
| ✅ |  | Absolute |



### ✅ `/test/asynchronizer.parsing.test.ts` **0.6s**  <!-- {docsify-ignore} -->


#### 🔹 [Asynchronizer](https://badcafe.github.io/asynchronizer)

| Status | Suite | Test |
| ------ | ----- | ---- |
| ✅ | parsing | Parse incoming message |
| ✅ | parsing | Parse nested Identity |



### ✅ `/test/types.test.ts` **0.569s**  <!-- {docsify-ignore} -->


#### 🔹 Advanced Jsonizer types

| Status | Suite | Test |
| ------ | ----- | ---- |
| ✅ | Code | Must compile |
| ✅ | Class | Extend dynamic class |



### ✅ `/test/graph.test.ts` **0.571s**  <!-- {docsify-ignore} -->


#### 🔹 Graphs

| Status | Suite | Test |
| ------ | ----- | ---- |
| ✅ | `JSON.stringify()` | Invariant |
| ✅ | `JSON.stringify()` | Invariant (realistic) |
| ✅ | `JSON.stringify()` | Customize `.toJSON()` |
| ✅ | `JSON.stringify()` | Auto-discard the unwanted field |
| ✅ | `JSON.parse()` | `ReferenceError` |
| ✅ | `JSON.parse()` | 👍 |



### ✅ `/test/errors.test.ts` **0.545s**  <!-- {docsify-ignore} -->


#### 🔹 Errors

| Status | Suite | Test |
| ------ | ----- | ---- |
| ✅ | reviving | Error |
| ✅ | reviving | TypeError |
| ✅ | reviving | MyError |
| ✅ | reviving | MyWarning |
| ✅ | reviving | 503 Service Unavailable |
| ✅ | reviving | null |
| ✅ | naming | Class.rename() on existing class |



### ✅ `/test/case.rebolon.test.ts` **0.618s**  <!-- {docsify-ignore} -->


#### 🔹 Use case (taken from another tool)

| Status | Suite | Test |
| ------ | ----- | ---- |
| ✅ | https://github.com/Rebolon/json-reviver | Revive wrapped book |
| ✅ | https://github.com/Rebolon/json-reviver | Revive book |
| ✅ | https://github.com/Rebolon/json-reviver | Revive books |



### ✅ `/test/case.emmkimme.test.ts` **0.587s**  <!-- {docsify-ignore} -->


#### 🔹 Use case (taken from another tool)

| Status | Suite | Test |
| ------ | ----- | ---- |
| ✅ | https://github.com/emmkimme/json-helpers | Revive busEvent |
| ✅ | https://github.com/emmkimme/json-helpers | JSON.stringify -> JSON.parse |



### ✅ `/test/class.test.ts` **0.453s**  <!-- {docsify-ignore} -->


#### 🔹 Class

| Status | Suite | Test |
| ------ | ----- | ---- |
| ✅ | rename() | w/o ns |
| ✅ | rename() | with @Namespace |
| ✅ | Inherit | Parent class is also the namespace |
| ✅ | Library loaded multiple times | Duplicate |
| ✅ | Library loaded multiple times | Deduplicate |



### ✅ `/test/replacer.test.ts` **0.497s**  <!-- {docsify-ignore} -->


#### 🔹 Replacer

| Status | Suite | Test |
| ------ | ----- | ---- |
| ✅ |  | Capture without JSON.stringify() |
| ✅ |  | replacer() recursive |



### ✅ `/test/destructure.test.ts` **0.509s**  <!-- {docsify-ignore} -->


#### 🔹 Destructuring

| Status | Suite | Test |
| ------ | ----- | ---- |
| ✅ |  | Invariants |
| ✅ |  | [Jsonizer.toJSON](): string |
| ✅ |  | toJSON(): string |
| ✅ |  | [Jsonizer.toJSON](): object |



### ✅ `/test/emptyKey.test.ts` **0.37s**  <!-- {docsify-ignore} -->


#### 🔹 Empty object key

| Status | Suite | Test |
| ------ | ----- | ---- |
| ✅ | Stringify with empty key | as the first item |
| ✅ | Stringify with empty key | as the last item |
| ✅ | Stringify with empty key | as the single item |
| ✅ | Stringify with empty key | Invariant |
| ✅ | Parse with empty key | as the first item |
| ✅ | Parse with empty key | as the last item |



### ✅ `/test/asynchronizer.ns.test.ts` **0.333s**  <!-- {docsify-ignore} -->


#### 🔹 [Asynchronizer](https://badcafe.github.io/asynchronizer)

| Status | Suite | Test |
| ------ | ----- | ---- |
| ✅ | Unordered @Namespace() | with @Type() = on-the-fly classes |



