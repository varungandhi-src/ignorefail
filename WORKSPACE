load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

_LINGUIST_VERSION = "7.27.0"
http_archive(
    name = "com_github_linguist",
    sha256 = "3d2c2f5bce2af68a52bc300c2e4991145ad201826b0c73358e89127d85e30d0e",
    urls = ["https://github.com/github-linguist/linguist/archive/refs/tags/v%s.tar.gz" % _LINGUIST_VERSION],
    strip_prefix = "linguist-%s" % _LINGUIST_VERSION,
    build_file = "//third_party:linguist.BUILD",
    patches = ["//third_party:linguist.patch"],
)

_FORK_LINGUIST_VERSION = "a05ca8a4b0bc03b29a3e5f6808a586872ec657f9"
http_archive(
    name = "com_github_varun_linguist",
    sha256 = "9fb738b810018813692b99fa07bb21a44dbd0be31db3d6ef52498f03fb1b7c57",
    urls = ["https://github.com/varungandhi-src/linguist/archive/%s.tar.gz" % _FORK_LINGUIST_VERSION],
    strip_prefix = "linguist-%s" % _FORK_LINGUIST_VERSION,
    build_file = "//third_party:linguist.BUILD",
    # .bazelignore was added to my fork, so this patch isn't needed
    # patches = ["//third_party:linguist.patch"],
)
