load("//tools/build_defs/oss:soloader_defs.bzl", "android_aar", "export_file")

android_aar(
    name = "soloader",
    manifest_skeleton = "AndroidManifestSkeleton.xml",
    deps = [
        "//java/com/facebook/soloader:loader_for_aar",
    ],
)

export_file(
    name = "nativeloader",
    src = "//java/com/facebook/soloader/nativeloader:nativeloader",
    out = "nativeloader.jar",
)

java_library(
    name = "annotation",
    deps = [
        "//java/com/facebook/soloader:annotation",
    ],
)
