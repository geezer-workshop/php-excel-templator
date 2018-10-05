# PHP Excel Templator

[![Latest Stable Version](https://poser.pugx.org/alhimik1986/php-excel-templator/v/stable)](https://packagist.org/packages/alhimik1986/php-excel-templator)
[![Latest Unstable Version](https://poser.pugx.org/alhimik1986/php-excel-templator/v/unstable)](https://packagist.org/packages/alhimik1986/php-excel-templator)
[![License](https://poser.pugx.org/alhimik1986/php-excel-templator/license)](https://packagist.org/packages/alhimik1986/php-excel-templator)
[![Total Downloads](https://poser.pugx.org/alhimik1986/php-excel-templator/downloads)](https://packagist.org/packages/alhimik1986/php-excel-templator)
[![Monthly Downloads](https://poser.pugx.org/alhimik1986/php-excel-templator/d/monthly)](https://packagist.org/packages/alhimik1986/php-excel-templator)
[![Daily Downloads](https://poser.pugx.org/alhimik1986/php-excel-templator/d/daily)](https://packagist.org/packages/alhimik1986/php-excel-templator)

[Инструкция на русском языке (Russian)](README_ru.md)

It's PHP Spreadsheet extension that allows you to export excel files from an excel template.
Using the extension you don’t need to create excel files from scratch using code, set styles and so on.

## Simple example
There is a simplest example of how this might look (using less code).
Suppose we have an excel file with the following template variables:
![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAApQAAABiCAIAAABh+dRGAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAIGNIUk0AAHolAACAgwAA+f8AAIDpAAB1MAAA6mAAADqYAAAXb5JfxUYAAAvhSURBVHja7N1rbFPnHcfxv7mUMnqhXQs0F9KkdrlsjIFGi01LRsOAZFTlslDaTSvRil00tSS7kLZqtFapVkHp7AmpKGZLI7ZClowGVZPdRM16gdgradlQ2QzYgwYnZWtR+6KTaKXYZy+ci2Ns5xjbxOfk+xEvMDjPec7/POf55Tk+tg2P7W7b+/N1gnHA+8/zh94+ecMNN980ffq0r10nIhMNut3Zv/39fQY2AL0yPLa7jSoAAKAhk0SEBQoAABoLbxE5deFLagEAgCZMoAQAAGhv5b3tpcMUAgAAzYT3XfOLMtjcD1ctpKYAEnm14wSzRLZ91WCesnIbddDksXtz7xSbV+3K++5vGdPfpP/TyZ9d8IXCYaoPIAlmiatACfdTBH2fIAM3rJ386FKa25sybbKIhMMKpQeQBLPEVUlvwlvnJ8gkTksAhLfeslsJUQTCm9MSALOEZkwQES6bE95JFN06pefTr0ZsVeG0BJB0bmKWyH54s/LW/Qly5eFdeMs1i4qnxYY3v1Nj0FH7mtp3pPypN565m2JAc7NE8NXqrS9/NPTwvp2Hd9yjoSrr9TXv//o3v3DmdOTveXe27TDdzso7JQVfn/ztoqmhUEibpyWuAu9b75SsKRW3x/P0EjPlgNZmCUVRxPQjZ+OGQpHggRprrf2eI9u1M5LDelx5nzyxqPGL7U+uaZ4hIvLRm0ef7JjZvHIa4a1W/k2TFhRc298f1uxpiezrPvpG0fI/bpB/bz969PGlFgoCrc0Siogokd4WLLunZO/R8z3hpYVaWXjrcOX9ya8aL9y/ZeUjt/ZHrisXlS09qMc9zVZ43zZ94vy8a/r7Q5o+LZFtHs9fjZaG/Ntkxeym3x96cOn6AmoCba28w4ooYSUcVkR63z1y1risNj+saOYt6vp7zfuTL87IzG3fDInCCZJ6eM+6ccLcWZP6QwmHRUjh4xcg0vfnV44Ur/hNXkgRy7JiZ5enZ90PSG9oapYIKyKBg7YVByMPi7dW52loftPhh7T853+nRZRwv8IJkmp4z7jeYJoxIUlys/JGRPDYu4HZ9z51mxIOS9537r3j4LtHejc+mEdhoKmVt8gdm1/e+0CBiMj79lU/eyL80m81M4x1eLe5otP9yvLK+9br5I5bJNHVcsIb0evurq5zEjz3k4f2D//be72VD+RTGmhollAUkfBgbxdbVspbPb1KeJZGgk5/r3nPn75WAp0nS+79BieI6vC+ZZpSfLOEQnFbNBDeGOGDlsbg7VU7HZWDa5Te16utLS3e+6t5yxg0tPJWRBRFGejtB11vyu1VsxTNfC67Du82v7Hqe1M3/uHD4ur5j8wQEel5619PS/GrK6YS3vHdPDU8+8Zwf7+qFghvvHfsbbE8tTFqmstb+9B9rS8ceX/7ksWUB1oK77OtP61oHXh83/a2jRoKbz2+z7vou3cektMbHR/siTyeOevQE5OFu83juunaUMH1/f39alvgs5OwxPra67EjYUl102uR23cBjcwSeRvqX9swMg81NID1+glrs0uN3aXR+xlSxusJMkp4f/7lxM+/nKi736kBsPLWd5X5bPPxvfLmtATALKE5fLa5RhlSCm//p5Mj38bNaQmA8NZFerPyHgcr788u+DK11W5/H6UHwCwxhopEDCd91EHfJ4ih9+KlTG2y45ivqnwRpQeQyIlTHy+cy+f1UGSke+wmUCwAALSF8AYAgPAGAACENwAAILwBANBveAfbtpVVrra1BSkWAAC5H97enZWrn5cfby2iUAAA5IrkH49qrm1tFwk2d1EoAAC0sfIGAACENwAAILwBACC8AQAA4Q0AADIk+d3m3p2Vz3ZE/trzaNkBMT78u4b1hVQNAICcDW9zbWt7LUUCACCXcNkcAADCGwAAEN4AAGCIodF1PIPNLS6eSU0BAMhuePdevJSptjqO+arKF1FTAImcOPXxwrl51IEiI81jx2VzAAA0hvAGAIDwBgAAhDcAANBbeLttBoPBYHNrrdMWRyDNRgIOi8GQgXbGgYSDJCMHIncwJADCO9i2raxydeTPzu5U549ho8ZqwGFJI3vdh51mu19pKB/rOTOjvz6oatBY7VFcVm/LXwLZOjS5VpYr3cSYDZKrXYGUhwQAnYV3X/PzXaVNre2dre1ND5d07NrlSaVps92vRLiszopsrwQWzDFyNHPz0OQOBgmA8RDe+Zsbdm+OfIlY4V2lRjl3vu+KNlLeoLis3poX3Zet/WzugcemGq84K6Ku9kUvEIeXLW6biuuB8dof0cRAC26bweJw2AafGPMwUR8irUUuwQ71N+4uJO+bxXF6lD6rrElaYg5Nwl22OAIxuxy32zFVtVhi9yKmKZt7uInosqVV+RQHycgDoYsKANC/3ouXVP1xPzdnxXMtSZ/T6Do+sJ5T/HZz1PIussQTsboURXFZB/8j+kl+uzny3zHPjnmayyox7Q78a/RaUqKebrb7Y9oefrLLKjK8mdiHifrgt5uH166xz4nahXhid2W4mTRqomrL8fsQ27CaXfbbzcNPj9Pt2DKO7FykqcjjyN+jHkSXJo3KqxgkiQ6ETiqQ4pC4qv7h61NAkZH2sVMZ3md2b1n+/X1nejMQ3vFnmBGTTexPj5h3lWSTctztJAvvBOGYpA+JWlMxX14eMpfv1pXWJGmN1IW3yl2Ou6nhp8QegMuja8Q+jfjdyerKUuVjupxoh/RVAdVDglwhvKG9Y6fqbnPPnkf3SdUz6wszstYfviBoqvEmfJa3xjR02bDCmfzCb53PFH250DzPlJmrEqr7oJLf581OTdw2Q/08v6faKEmu5mZyl70+v/pu50DlYwZJ4gOhmwpcPiQAjJvXvAeSe3VdT1XT4IvfV8h92CnWdeUibpupZoEr+gpifDHriKSzUPk668BcGj2vpi+VPqhhmmdOMNGmV5PA6Q/Nm9aO6Jyx2jP4tNFurx46NCnssnmeSX23c6DyMYMk0YHQTwXiDAkA4ye8g82/yERyBxyWCqfZ/suYFHG/OHKx8uHpgYWRce0ms7M+3q03o9+LVL7OKkM/67ZZHAExzlkgzsPuoZ6o6nPiPiQztAvx25yzYKhvCXpyBTVJvpBM4dAk3WVnhWWw4/XOy3IhttsplSXTlR99kCQ6EHqpQFpDAoDmw7v74L4ekZ5Xtgy+1btsTwpTwvCFP1PLJv/g2qG8wWV1VhgMBoOhfp7dGj1feWtMA7Ousdrj39QyfN0wlZtoyxv8dhnYdP28/dXG6G2afHUuq8oZNNU+jNyF0fpm8tUNrdWyXhN1hybpJqyuOl+k4zULXJEfSNDt1MtyFSqv7kCMowoA0DZ9fCXoOH+BL9u7H3BYTL66Mf4MnDGtkuYqkLtnBN9WSZGRkWOnj49HLV9n9daYxuWqI+CwGCqcvL7JIGFIAOPJJJ1MzA2K0pBT6544L2ib7VlYChmrPUo141iDgyRrGBIA4Q1iIpIG4/uAUgEAucXQ6DqeweYWF8+kpgAAZDe8dXHDGgBt4F4qioyMHLsJFAsAAG0hvAEAILwBAADhDQAACG8AALRqlPd5B9u2bTlwVkREyupbd1goGAAAub3y9h7oKm1qbe9sba9f3lm3hy8qAgAg18PbXDv4ZaCFBSXS0xOkYAAA5HZ4Ry3BD5w1LltWSMEAABhro322efeusl2dIiLLn+1cT3YDAJD7K+8lOzpb2ztb25sK9pdV7vJQMAAAcj28BxXeVWqUc+f7qBgAALkc3n3NtsE7zIPH3glI8ex8KgYAwBhL+pp3/rIVPY+WVUYelGx18D5vAAByPLylcPPu9s0UCQCAXMLHowIAQHgDAADCGwAADDE0uo5nsLnFxTOpKQAA2Q3v3ouXMtVWxzFfVfkiagogkROnPl44N486UGSkeey4bA4AgMYQ3gAAEN4AAIDwBgAAhDcAALoOb8+e1WWVq21tQeoFAIAWwrt7V11P2aoiagUAgDbCO9j8p85VDz5EdgMAoI3wDrb9el/Rs7VLKBQAAJoI777m5w8U1z9upkwAAOSOJN/nHWy2v1Kyo91CkQAAyCX/HwCeoqUoPtouzgAAAABJRU5ErkJggg==)
The code will be as follows:
```
use alhimik1986\PhpExcelTemplator\PhpExcelTemplator;

PhpExcelTemplator::saveToFile('./template.xlsx', './exported_file.xlsx', [
	'{current_date}' => date('d-m-Y'),
	'{department}' => 'Sales department',
]);
```
As a result, we get:
![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAp0AAABaCAIAAAB1xXpMAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAIGNIUk0AAHolAACAgwAA+f8AAIDpAAB1MAAA6mAAADqYAAAXb5JfxUYAAAxzSURBVHja7N1/bBvlGcDxx6WlVB3ix6At+dGQYtMfW9a1WqF2ga6ka7EVRH8soWVTIRq1V02j9jRaQERDChJqYbNRJVDMFqputCEZpELIJhUZg7a2aAGpSjVT7LWkTssGCP5gUkFKfPvj7NhJ7mwncdre5ftRJRrqe+/18/re5573zhfLr5/rFAAAYApTb1tUVcLmfrFmMTEFoOeVQyeYJSbady326au3EQdDjt3bL073RMeb10Xk9h9Zx9+b+BfTvvosNpBKMTAA8mCWuAiUVD9BmLQHyFT1Pyc/vTDOhqbPnCYiqZTCqADIg1nioiR28vrkPUCmcsQCIK+bLa0rAwSBvM4RC4C8bgZTRIR1ePL62FTdOL33i++GdEjhiAWQd9pilpj4vE69PpkPkLHn9cobrlxSPXN4XudMHBlH/PfsfFecj7/15O0EA4abJZKveLe+8Ongj3fvOrjjDgNF2azX1/8b3/TMJ6fUv5fd2rnDdjMHSKnyesX3p/24asbAwIAxj1hcBNF33p13z0oJRyJPLLMTDhhtllAURWy/DLZuqBRJ7ve5d/rvOLzdOJ/klBnr9ZMnlrR+s/2xe9pmiYh8+vaRxw7Nbls9kwOkBHm9/LqpNRVX9fenDHvEYuIdP/JW1V1/2yD/3n7kyG+XOwgIjDZLKCKiqL2tWHHHvBePnO1NLa80Srluwnr98z+0fnbvQ6sfvLFfXaiuql1+wIzv9BLk9ZuuvWJR2ZX9/QOGPmIx0SKRf1gdLeU3yaq5e//y2v3L11cQExirXk8poqSUVEoR6Xvv8Gnrip3lKcUwX7033/X1z7/5RGZv++GAKBwgJc3rc66ZsmDO1P4B3U/MgMITJyBy7u8vH65e9aeyAUUcK6qDRyO9635OYoehZomUIpI44Fl1QP2xequ3zEDzmwmfS/Of/50SUVL9CgdICfP6rKsttllT8iR16nWoksfeS8y98/GblFRKyn5y5y0H3jvct/H+MgIDQ9XrIrdseuHF+ypERD7wr/ndI6k/Pm+Yj7EJ74dXTPq+Ll29fuP35JYbRG/5nbyO3Gr96NEzkjzzq837sv/v/b76+8oJDQw0SyiKSCrT26WO1fJOb5+SmmOQHGi+6+uLrq2TRPfJeXf+gAOkFHn9hplK9fUyMKC5Mwt5HUN82N6avLlxV6A+U9n0veF1t7dH7/XyfTcYqF5XRBRFSff2w6Nvy82NcxTDPNvehPfDX9P4sxkb/9pT7V304CwRkd53/vWEVL+yagYHyKjz+vUzUnOvSfX3F9UCeR3vH/unOB7fmDMDltVtvrvjmcMfbF+2lPDASHn9dMdvXB3pn+/e3rnRQHndjN9fr/rpra/JqY2BD/eoP8+e89oj04T74Ueb16+7aqDi6v7+/mJb4ElSWOZ+/Y3hn4Rl3r2vqzcYAwaZJco2NL++YWiqNNAH2KzPm5u70np8Ze77HFA4QEab17/+9oqvv73CdGfiAKjXzR1lng9Pvc4RC4C8bhY8H96gLKXK6/Evpqm/PZ0jFgB53RSJnXp9ctfrX30WK1WHjsfPMSoAmCUuoSoRy8kYcZi0B4il78sLperNoWOxRucSRgWAnhMfn1+8gEcUEWRM4NhNIY4AAJgGeR0AAPI6AAAgrwMAAPI6AAAoRV5Pdm6rrV/r6UwSLAAADJ3Xo7vq1z4tW7ZWESgAAAwg/3Nk7Ts7ukSSbUcJFAAAhq/XAQAAeR0AAJDXAQAAeR0AAJDXAQAwl/z3w0d31T91SP1r78O1+8X6wJ9b1lcSNQAAjJjX7Ts7unYSJAAADIJ1eAAAyOsAAIC8DgAAJo6lNfRRCZtbWj2bmAIAcMnyet+XF0rV1qFjsUbnEmIKQM+Jj88vXlBGHAgyJm7sWIcHAMA8yOsAAJDXAQAAeR0AAJDXgQLCHovFEy5ZW45AgpgCMF9eT3Zuq61fq/7Zdbz4ZhMBhyVXwfk2EXCMfVLO2duwNsIei8WSb4pWNx3yAv3WNN9e9jU6G2rsQu2WpUDfxhnScRrXiJRwFzmxmui3fNFcLrEFMOny+rm2p4+u3NvR1d3RtfeBeYd2746Mpmm7P66oQu6ga+Lqn7DH5hN1XyF30JWzn7DH1eN22/NljC3S5LcX11rOlLmlvUF9b3G/PehSp0/NDXV24erxZ7YX35biA3OxQno5JUBX0B1Kv2dppoYGgPHk9fJNLc9tUn99W+VtK61y5uy5Me3E2aKE3FHfs2HtujYRcFhsvqgEXTn1q3ZJHPaMqHDDB4PibvJaRUScj/rt0Vg8s5vmoLvp0YX5uqVEvDYpqrUcVm8kor5CrHUNduk5ldDbUGsXiVM9UjM/vf38GilFSLXDlQg4HIHEYMGbEziNpYWwx+IIBNTXOhzDR2RYU55wtonc8dDrhsUTHtYNjUHXGFwREftCW+Y9Z8JexJpKwSWVEXvK/psjcKpgUwaLLQDy+gjnzyakem75WPfjXOeW4MGwiIQ9W2TfYLHbHEiI1RtR4n67uEOKoqhTd9hj89Wky7S4v8elPzklTvVkZ34RETXNSiKwxVcTanGOsj7UaU1XPBaVmvnW0Wxo9Ta5g6709O3q8e/LJKsxhzRPuKI+W/PCeGZpwJZZWhg+BJkX+ySkKIoSiYwYEZGoz3Zw3eAihcUWaxq+4pBn1IKudDcyZyMag64Vq7oGe9RnG34qp9P/oasuI3uifibSKx7D9pkIbMkstyhNMV+wQFMmiC2AyZ3Xk22vdlsf2OwowR6zVZe1rkGzHpZEoDlo9z/qzObBaPubiWyJrT9RZerfsWV1vdb0TwOGdLToDZ0t6jq6zSdjzupFhUtE3KF0vKzeJnf6ZEN3CNx5Q5b5V2tdgz37w/waUVsorhvOdW69Ux6twbV6I0rIHfXZcivPQh+hfD1JnwmNiOGb7dHMcos4W0Juk8UWAHl9iMieh1+SxifXV5Zkl9n1RJsvqvsqdSpXuYKjqbdF4ppZvYj74TRb091QvaKulZjTG+oIeyyWdHXW0G4b9U174wlXOs8UNwRjMLZRK3gmOFgTp2NVRP+1emL1RuL+HpfWKnw8Fp2UsQUwGfN6ZM/apt7GvZkL7WMUPhgU9zrn8PVEe54CRsmlv1I7WNNk1MyXWPraYnpyjfpsFkdAvJFMa7qVk1ZrVqvWhmGPxdXjjw8WZ1obFqyurd59fntO5aXWp4U6OTykowiXfaGt+CEYg2JHbSyLJ9596bsWiuq/Tk/S8Q3VZNbN02wLx/1RNHBsAUyevJ5s+30pknoi4HBprFeHnx1a0AwuIVrrGrQvm2rdWpVzmVnCz/qi7nVOtcDLTq52f7zYaVCjNe0Vh9ykXvSGI84AEm+2R3XPAIoNqX64RGTwlv5EoDlob6iz5h2CYUa1qJu3G8XsYuTgqneU5fR16C0Mev0v3JMRadw6v0YymyQCjsF62CyxBUBeFxGR4wde6hXpffmhzFfYa/eMYmUxu25oa28YTKzOlpA7XUs3L/S7cyeuqM+Wntit3ki8oT277Jj3pl5nS2Zx1eLq8ceLv6iu3kWcKejTOymiNXXCzl0W9YR1NtTaRU4ELDafjKbH2iHNGy53qClmU3dVk74OqzMEGqkkOyLFVdSjGLWidmH17ss2OHgmVbj/Oj3JfhXeNuI6jbMl7hc1vLZYU7bUNm1sAZgVv6fVxBIBhy3WpIz39kEQ29LhV4gSZEz02PEcWQAAzIO8DgCAeUwlBOZl9UYUokBsAUwqltbQRyVsbmn1bGIKAMAly+vcNwfgouGWLoKMiR47rq8DAGAe5HUAAMjrAACAvA4AAMjrAACgsALfX092bnto/2kREalt7tjhIGAAABi2Xo/uP7pyb0dXd0dX813dTXuixAsAAOPmdfvOzG9orayYJ729SQIGAIBh83pO4b7/tHXFikoCBgDAZazQ8+GP767d3S0ictdT3etJ6wAAGLpeX7aju6Oru6Nrb8W+2vrdEQIGAICB83pG5W0rrXLm7DkiBgCAQfP6uTZP5h745LF3E1I9t5yIAQBw+cp7fb18xareh2vr1R/mbQ3w/XUAAIyb16Vy03NdmwgSAAAGwXNkAQAgrwMAAPI6AACYOJbW0EclbG5p9WxiCgDAJcvrfV9eKFVbh47FGp1LiCkAPSc+Pr94QRlxIMiYuLFjHR4AAPMgrwMAQF4HAADkdQAAQF4HAAAlyuuRPWtr69d6OpPECwAAg+f147ubemvXVBErAAAMn9eTba92r7l/M2kdAIDL3/8HAKsrZ/Qjly9UAAAAAElFTkSuQmCC)

Using this extension, we just create a template file with the styles we need and specify template variables in it. In the code, we just pass the parameters to template variables.

## Features
- We can insert several template variables in one table cell (if the data type is "string")
- We can insert a one-dimensional array, in this case additional rows will be created in the table
- We can insert a two-dimensional array, in this case the respective columns and rows are created in the table
- By specifying the value in the cells, you can change the styles of these cells, even when inserting arrays
- We can apply the same template on several sheets of the table

Features demo and usage examples are given in the folder "samples".

## Restrictions:
- Possible so-called side effects when using one-dimensional or two-dimensional arrays  in one sheet. Especially when it is located asymmetrically. An example of side effects is also given in the folder "samples".

## INSTALLATION:

```
$ composer require alhimik1986/php-excel-templator
```

### Template variable naming rules
The rules can be any, but I can offer my recommendation for naming template variables:
- {var_name} - for string values
- [var_name] - for one-dimensional arrays
- [[var_name]] - for two-dimensional arrays


### How to insert a one-dimensional array, so that the table create columns, not rows?
To do this, instead of a one-dimensional array, insert a two-dimensional one as follows:
```
$param['[[var_name]]'] = [['text 1', 'text 2', 'text 3']];
```

## Using setters
In the example above, the minimum code without setters was used.
The data types (for example: a string, a one-dimensional array, or a two-dimensional array) in this code is automatically recognized and the necessary setter is chose.
But if we want to use a specific setter, the same code will look like this:
```
use alhimik1986\PhpExcelTemplator\PhpExcelTemplator;
use alhimik1986\PhpExcelTemplator\params\ExcelParam;
use alhimik1986\PhpExcelTemplator\params\CallbackParam;
use alhimik1986\PhpExcelTemplator\setters\CellSetterStringValue;

$params = [
	'{current_date}' => new ExcelParam(CellSetterStringValue::class, date('d-m-Y')),
	'{department}' => new ExcelParam(CellSetterStringValue::class, 'Sales department', function(CallbackParam $param) {
		$sheet = $param->sheet;
		$cell_coordinate = $param->coordinate;
		$sheet->getStyle($cell_coordinate)->getFont()->setBold(true);
	}),
];
PhpExcelTemplator::saveToFile('./template.xlsx', './exported_file.xlsx', $params);
```
At the moment the extension has 3 kinds of setters:
- CellSetterStringValue (for string values)
- CellSetterArrayValue (for one-dimensional arrays)
- CellSetterArray2DValue (for two-dimensional arrays)

You ask, what for specify setters explicitly?
- First, because it's flexible: let's say you want to create your own setter with your own algorithms that eliminate the side effects, which I mentioned above.
- Secondly, in each setter, you can pass a callback function in which we can change the styles of the inserted cells. For example, you need to highlight with bold font the employees who made the best sales in this month.

Examples of code that uses all kinds of setters are listed in the folder "samples".
