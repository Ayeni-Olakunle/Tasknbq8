<template>
    <div>
        <b-container fluid class="bv-example-row">
            <b-row>
                <b-col sm="2" class="navbar">col-sm-8</b-col>
                <b-col sm="10" class="holdAll">
                    <div class="topHeader">
                        <div>
                            <b-icon icon="border-width" aria-hidden="true"></b-icon>
                        </div>
                        <div class="iconName">
                            <span class="iconKonia"><b-icon icon="bell" aria-hidden="true"></b-icon></span>
                            <span class="iconKonia"><b-icon icon="envelope" aria-hidden="true"></b-icon></span>
                            <span class="iconKonia">Ayeni</span>
                        </div>
                    </div>
                    <div class="topHeader secondTop" style="border-bottom:none; background-color: transparent;">
                        <div>
                            <p>Hello Welcome Here</p>
                        </div>
                        <div>
                            <p>Dashborad/Home</p>
                        </div>
                    </div>
                    <div class="holdProptyMar">
                        <div class="holdPropty">
                            <div class="propty">
                                <p>Total Completed</p>
                                <h3>$8500</h3>
                                <div>
                                    <b-progress :value="45" :max="max" class="mb-3" variant="success"></b-progress>
                                </div>
                            </div>
                            <div class="propty">
                                <p>Income Details</p>
                                <h3>$7800</h3>
                                <div>
                                    <b-progress :value="30" :max="max" class="mb-3"></b-progress>
                                </div>
                                
                            </div>
                            <div class="propty">
                                <p>Task Completed</p>
                                <h3>$500</h3>
                                <div>
                                    <b-progress :value="25" :max="max" class="mb-3" variant="warning"></b-progress>
                                </div>
                            </div>
                            <div class="propty">
                                <p>Task Completed</p>
                                <h3>$650</h3>
                                <div>
                                    <b-progress :value="30" :max="max" class="mb-3" variant="danger"></b-progress>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div>
                        <b-row>
                            <b-col sm="7" class="graph">col-sm-8</b-col>
                            <b-col sm="4" class="graph">col-sm-4</b-col>
                        </b-row>
                    </div>
                    <div>
                        <b-row>
                            <b-col sm="4" class="graph">col-sm-8</b-col>
                            <b-col sm="7" class="graph">
                                <p style="text-align: left; paddind: 10px;">New Order</p>
                            </b-col>
                        </b-row>
                    </div>
                      
                </b-col>
            </b-row>
        </b-container>
    </div>
</template>

<script>
export default {
    data() {
      return {
        value: 33.333333333,
        max: 50
      }
    }
    
}
</script>

<style scoped>
.holdAll{
    /* margin: 0;
    padding: 0; */
}
.topHeader{
    display: flex;
    justify-content: space-between;
    align-items: center;
    border-bottom: 1px solid lightgray;
    background-color: white;
    padding: 5px 25px;
}
.iconName{
    display: flex;
    justify-content: center;
    align-content: center;
    padding: 10px;
}
.iconKonia{
    margin-right: 20px;
    margin-top: 10px;
}
.secondTop{
    border-bottom: medium none;
    margin-top: 20px;
    margin-bottom: 20px;
    color: gray;
    font-size: 15px;
}
.holdProptyMar{
    margin-bottom: 20px;
}
.holdPropty{
    display: flex !important;
    justify-content: space-around;
    align-items: center;
}
.propty{
    width: 25%;
    height: 150px;
    background-color: white;
    border: 1px solid lightgray;
    border-radius: 5px;
    margin: 0px 10px;
    padding: 20px;
}

.graph{
    background-color: white;
    height: 300px;
    margin-bottom: 20px;
    border-radius: 5px;
    margin: 20px;
}
.navbar{
    background-color: #1c0080;
}
</style>