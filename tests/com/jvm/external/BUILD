load("//:defs.bzl", "artifact")

java_test(
    name = "ArtifactExclusionsTest",
    srcs = ["ArtifactExclusionsTest.java"],
    test_class = "com.jvm.external.ArtifactExclusionsTest",
    deps = [
        artifact(
            "com.google.guava:guava",
            repository_name = "exclusion_testing",
        ),
        artifact(
            "junit:junit",
            repository_name = "regression_testing",
        ),
        artifact("org.hamcrest:hamcrest"),
        artifact("org.hamcrest:hamcrest_core"),
    ],
)

java_test(
    name = "GlobalArtifactExclusionsTest",
    srcs = ["GlobalArtifactExclusionsTest.java"],
    test_class = "com.jvm.external.GlobalArtifactExclusionsTest",
    deps = [
        artifact(
            "com.diffplug.durian:durian-core",
            repository_name = "global_exclusion_testing",
        ),
        artifact(
            "junit:junit",
            repository_name = "regression_testing",
        ),
        artifact(
            "com.google.guava:guava",
            repository_name = "global_exclusion_testing",
        ),
        artifact(
            "com.squareup.okhttp3:okhttp",
            repository_name = "global_exclusion_testing",
        ),
        artifact("org.hamcrest:hamcrest"),
        artifact("org.hamcrest:hamcrest-core"),
    ],
)

java_test(
    name = "HasherTest",
    size = "small",
    srcs = ["HasherTest.java"],
    test_class = "rules.jvm.external.HasherTest",
    deps = [
        "//private/tools/java/rules/jvm/external:hasher",
        artifact(
            "junit:junit",
            repository_name = "regression_testing",
        ),
        artifact("org.hamcrest:hamcrest"),
    ],
)

java_test(
    name = "JsonArtifactsTest",
    srcs = ["JsonArtifactsTest.java"],
    test_class = "com.jvm.external.JsonArtifactsTest",
    deps = [
        artifact(
            "io.quarkus:quarkus-maven-plugin",
            repository_name = "json_artifacts_testing",
        ),
        artifact(
            "org.json:json",
            repository_name = "json_artifacts_testing",
        ),
        artifact(
            "junit:junit",
            repository_name = "regression_testing",
        ),
    ],
)

java_test(
    name = "NeverlinkTest",
    srcs = ["NeverlinkTest.java"],
    test_class = "com.jvm.external.NeverlinkTest",
    deps = [
        artifact("com.google.guava:guava"),
        artifact(
            "junit:junit",
            repository_name = "regression_testing",
        ),
        artifact("org.hamcrest:hamcrest"),
    ],
)

java_test(
    name = "UnsafeSharedCacheTest",
    srcs = ["UnsafeSharedCacheTest.java"],
    tags = ["manual"],
    test_class = "com.jvm.external.UnsafeSharedCacheTest",
    deps = [
        "//tests/integration:guava_import",
        artifact(
            "junit:junit",
            repository_name = "regression_testing",
        ),
        artifact("org.hamcrest:hamcrest"),
        artifact("org.hamcrest:hamcrest-core"),
    ],
)
