CXXFLAGS := -std=c++1y -Isrc/include
LDFLAGS  := 

SRCS     := $(wildcard src/*.cpp)
EXECS    := $(SRCS:src/%.cpp=%)

.PHONY: clean

$(EXECS): %: src/%.cpp
	$(CXX) $(CXXFLAGS) $(LDFLAGS) $< -o $@

clean:
	rm -f $(EXECS)
