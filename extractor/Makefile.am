bin_PROGRAMS = compile run_extractor

noinst_PROGRAMS = \
  binary_search_merger_test \
  data_array_test \
  intersector_test \
  linear_merger_test \
  matching_comparator_test \
  matching_test \
  matchings_finder_test \
  phrase_test \
  precomputation_test \
  sampler_test \
  suffix_array_test \
  veb_test

TESTS = sampler_test
#TESTS = binary_search_merger_test \
#  data_array_test \
#  intersector_test \
#  linear_merger_test \
#  matching_comparator_test \
#  matching_test \
#  matchings_finder_test \
#  phrase_test \
#  precomputation_test \
#  suffix_array_test \
#  veb_test

binary_search_merger_test_SOURCES = binary_search_merger_test.cc
binary_search_merger_test_LDADD = $(GTEST_LDFLAGS) $(GTEST_LIBS) $(GMOCK_LDFLAGS) $(GMOCK_LIBS) libextractor.a
data_array_test_SOURCES = data_array_test.cc
data_array_test_LDADD = $(GTEST_LDFLAGS) $(GTEST_LIBS) libextractor.a
intersector_test_SOURCES = intersector_test.cc
intersector_test_LDADD = $(GTEST_LDFLAGS) $(GTEST_LIBS) $(GMOCK_LDFLAGS) $(GMOCK_LIBS) libextractor.a
linear_merger_test_SOURCES = linear_merger_test.cc
linear_merger_test_LDADD = $(GTEST_LDFLAGS) $(GTEST_LIBS) $(GMOCK_LDFLAGS) $(GMOCK_LIBS) libextractor.a
matching_comparator_test_SOURCES = matching_comparator_test.cc
matching_comparator_test_LDADD = $(GTEST_LDFLAGS) $(GTEST_LIBS) libextractor.a
matching_test_SOURCES = matching_test.cc
matching_test_LDADD = $(GTEST_LDFLAGS) $(GTEST_LIBS) libextractor.a
matchings_finder_test_SOURCES = matchings_finder_test.cc
matchings_finder_test_LDADD = $(GTEST_LDFLAGS) $(GTEST_LIBS) $(GMOCK_LDFLAGS) $(GMOCK_LIBS) libextractor.a
phrase_test_SOURCES = phrase_test.cc
phrase_test_LDADD = $(GTEST_LDFLAGS) $(GTEST_LIBS) $(GMOCK_LDFLAGS) $(GMOCK_LIBS) libextractor.a
precomputation_test_SOURCES = precomputation_test.cc
precomputation_test_LDADD = $(GTEST_LDFLAGS) $(GTEST_LIBS) $(GMOCK_LDFLAGS) $(GMOCK_LIBS) libextractor.a
suffix_array_test_SOURCES = suffix_array_test.cc
suffix_array_test_LDADD = $(GTEST_LDFLAGS) $(GTEST_LIBS) $(GMOCK_LDFLAGS) $(GMOCK_LIBS) libextractor.a
sampler_test_SOURCES = sampler_test.cc
sampler_test_LDADD = $(GTEST_LDFLAGS) $(GTEST_LIBS) $(GMOCK_LDFLAGS) $(GMOCK_LIBS) libextractor.a
veb_test_SOURCES = veb_test.cc
veb_test_LDADD = $(GTEST_LDFLAGS) $(GTEST_LIBS) libextractor.a

noinst_LIBRARIES = libextractor.a libcompile.a

compile_SOURCES = compile.cc
compile_LDADD = libcompile.a
run_extractor_SOURCES = run_extractor.cc
run_extractor_LDADD = libextractor.a

libcompile_a_SOURCES = \
  alignment.cc \
  data_array.cc \
  phrase_location.cc \
  precomputation.cc \
  suffix_array.cc \
  translation_table.cc

libextractor_a_SOURCES = \
  alignment.cc \
  binary_search_merger.cc \
  data_array.cc \
  features/count_source_target.cc \
  features/feature.cc \
  features/is_source_singleton.cc \
  features/is_source_target_singleton.cc \
  features/max_lex_source_given_target.cc \
  features/max_lex_target_given_source.cc \
  features/sample_source_count.cc \
  features/target_given_source_coherent.cc \
  grammar.cc \
  grammar_extractor.cc \
  matching.cc \
  matching_comparator.cc \
  matchings_finder.cc \
  intersector.cc \
  linear_merger.cc \
  matchings_trie.cc \
  phrase.cc \
  phrase_builder.cc \
  phrase_location.cc \
  precomputation.cc \
  rule.cc \
  rule_extractor.cc \
  rule_factory.cc \
  sampler.cc \
  scorer.cc \
  suffix_array.cc \
  translation_table.cc \
  veb.cc \
  veb_bitset.cc \
  veb_tree.cc \
  vocabulary.cc

AM_CPPFLAGS = -W -Wall -Wno-sign-compare -std=c++0x $(GTEST_CPPFLAGS) $(GMOCK_CPPFLAGS)