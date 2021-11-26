# min_max-ruby
# about maximum and minimum of array   Ratiorg got statues of different sizes as a present from CodeMaster for his birthday, each statue having an non-negative integer size. Since he likes to make things perfect, he wants to arrange them from smallest to largest so that each statue will be bigger than the previous one exactly by 1. He may need some additional statues to be able to accomplish that. Help him figure out the minimum number of additional statues needed.
def solution(statues)
    mm = statues.minmax      
    addStatues= Array.new(mm[1]-mm[0]){|x| x + mm[0]} 
    addStatues = addStatues - statues
    number = addStatues.length      
end

