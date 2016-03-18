#include <stdio.h>
#include <stdlib.h>

#define uint64 unsigned long long

void check(uint64 should, uint64 is);
uint64 recursive(int i);
uint64 iterative(int i);

int main(int argc, char** argv)
{
  if (argc != 3)
  {
    printf("Usage: %s <number> <result>\n", argv[0]);
    return 1;
  }

  int number = atoi(argv[1]);
  uint64 result = strtoull(argv[2], NULL, 10);
  if (number < 0)
  {
    printf("error: number < 0\n");
    return 1;
  }

  printf("recursive:    ");
  uint64 rec = recursive(number);
  check(rec, result);

  printf("iterative:    ");
  uint64 iter = iterative(number);
  check(iter, result);

  return 0;
}

void check(uint64 should, uint64 is)
{
  int ok = (should == is);

  if (ok)
    printf(" PASS\n");
  else
    printf(" FAIL\n");
}

uint64 recursive(int i)
{
    return -1;
}

uint64 iterative(int i)
{
    return -1;
}

