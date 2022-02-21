<!--DO NOT EDIT : this file has been generated-->

# Reports

> Code quality reports

## Metrics

<div class="chart-container" style="float:right; height:450px; width:450px">
    <canvas id="metricsChart"></canvas>
</div>

| Files | 7 | |
| ----- | -: | - |
| Lines of code | 1050 | (w/o comments) |
| Comments | 1006 | (+ 130 with code) |
| Empty lines | 136 | |
| **Total lines** | **2192** | (w/o tests) |
| TODO | 3 | lines |
| Tests | 2821 | (w/o comments) |

<script>
var ctx = document.getElementById('metricsChart');
var myChart = new Chart(ctx, {
    type: 'pie',
    data: {
        labels: ['Code', 'Comments', 'Empty', 'Tests'],
        datasets: [{
            label: 'Metrics',
            data: [1050, 
                1006, 
                136,
                2821
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

**✅ &nbsp; 0 problems**



## Tests

|   | Tests suites | Tests |
| - | ------------ | ----- |
| ❌ &nbsp; Failed | 0 | 0 |
| ✅ &nbsp; Passed | 10 | 160 |
| ✴ &nbsp; Pending | 0 | 0 |
| ☢ &nbsp; Error | 0 | |
| **Total** | **10** | **160** |




### ✅ `/test/errors.test.ts` **2.2s**  <!-- {docsify-ignore} -->


#### 🔹 Errors

| Status | Suite | Test |
| ------ | ----- | ---- |
| ✅ | reviving | Error |
| ✅ | reviving | TypeError |
| ✅ | reviving | MyError |
| ✅ | reviving | MyWarning |
| ✅ | reviving | 503 Service Unavailable |
| ✅ | reviving | null |



### ✅ `/test/basic.test.ts` **2.382s**  <!-- {docsify-ignore} -->


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



### ✅ `/test/readme.test.ts` **2.743s**  <!-- {docsify-ignore} -->


#### 🔹 README.md examples

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



### ✅ `/test/graph.test.ts` **0.861s**  <!-- {docsify-ignore} -->


#### 🔹 Graphs

| Status | Suite | Test |
| ------ | ----- | ---- |
| ✅ | `JSON.stringify()` | Invariant |
| ✅ | `JSON.stringify()` | Invariant (realistic) |
| ✅ | `JSON.stringify()` | Customize `.toJSON()` |
| ✅ | `JSON.stringify()` | Auto-discard the unwanted field |
| ✅ | `JSON.parse()` | `ReferenceError` |
| ✅ | `JSON.parse()` | 👍 |



### ✅ `/test/destructure.test.ts` **0.309s**  <!-- {docsify-ignore} -->


#### 🔹 Destructuring

| Status | Suite | Test |
| ------ | ----- | ---- |
| ✅ |  | Invariants |
| ✅ |  | [Jsonizer.toJSON](): string |
| ✅ |  | toJSON(): string |
| ✅ |  | [Jsonizer.toJSON](): object |



### ✅ `/test/reviver.test.ts` **0.916s**  <!-- {docsify-ignore} -->


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



### ✅ `/test/case.rebolon.test.ts` **0.512s**  <!-- {docsify-ignore} -->


#### 🔹 Use case (taken from another tool)

| Status | Suite | Test |
| ------ | ----- | ---- |
| ✅ | https://github.com/Rebolon/json-reviver | Revive wrapped book |
| ✅ | https://github.com/Rebolon/json-reviver | Revive book |
| ✅ | https://github.com/Rebolon/json-reviver | Revive books |



### ✅ `/test/case.emmkimme.test.ts` **0.406s**  <!-- {docsify-ignore} -->


#### 🔹 Use case (taken from another tool)

| Status | Suite | Test |
| ------ | ----- | ---- |
| ✅ | https://github.com/emmkimme/json-helpers | Revive busEvent |
| ✅ | https://github.com/emmkimme/json-helpers | JSON.stringify -> JSON.parse |



### ✅ `/test/emptyKey.test.ts` **0.327s**  <!-- {docsify-ignore} -->


#### 🔹 Empty object key

| Status | Suite | Test |
| ------ | ----- | ---- |
| ✅ | Stringify with empty key | as the first item |
| ✅ | Stringify with empty key | as the last item |
| ✅ | Stringify with empty key | as the single item |
| ✅ | Stringify with empty key | Invariant |
| ✅ | Parse with empty key | as the first item |
| ✅ | Parse with empty key | as the last item |



### ✅ `/test/types.test.ts` **0.287s**  <!-- {docsify-ignore} -->


#### 🔹 Advanced Jsonizer types

| Status | Suite | Test |
| ------ | ----- | ---- |
| ✅ | Code | Must compile |



