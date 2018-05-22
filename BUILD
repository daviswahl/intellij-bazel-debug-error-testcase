# stax_api is a transitive dependency of xmlbeans,
# but it doesn't seem related to the bug. I've included it here just
# so that it's easy to rule it out as an issue.

#java_library(
#    name = "stax_api",
#    exports = [
#        "@javax_xml_stream_stax_api//jar",
#    ],
#    visibility = [
#        "//visibility:public"
#    ]
#)

java_library(
    name = "xmlbeans",
    exports = [
        "@org_apache_xmlbeans_xmlbeans//jar",
#        ":stax_api",
    ],
    visibility = [
        "//visibility:public"
    ]
)


java_binary(
    name = "testcase",
    srcs = ["src/main/java/Testcase.java"],
    deps = [":xmlbeans"],
    main_class = "src.main.java.Testcase"
)


