```
program halt-checker
    will-halt(prgm): boolean
        // hypothetical logic to test if prgm would halt in a finite amount of time
    end
end

program fuckery
    check(prgm): void
        if halt-checker.will-halt(prgm)
            loop infinity
        else
            exit
        end
    end
end

fuckery.check(fuckery) // 😲
